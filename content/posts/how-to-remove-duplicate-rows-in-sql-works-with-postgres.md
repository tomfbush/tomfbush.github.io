---
title: 'How to remove duplicate rows in SQL (works with Postgres)'
date: Fri, 24 Apr 2020 13:05:49 +0000
draft: false
tags: ['Databases', 'duplicates', 'postgres', 'postgresql', 'sql']
thumbnail: "https://wiki.postgresql.org/images/3/30/PostgreSQL_logo.3colors.120x120.png"
aliases:
  - "/databases/how-to-remove-duplicate-rows-in-sql-works-with-postgres/"
---

Note to self more than anything, this snippet was handy for to remove duplicate rows in SQL, that crept into a Postgres database as a result of a dodgy join.

There are probably more than a couple of ways of doing this but the best example I came up with after reading around is:

```
DELETE FROM table_name  
WHERE ctid NOT IN (  
   SELECT min(ctid)  
   FROM   table_name  
   GROUP  BY field1, field2);
```

The reason this works revolves around the `ctid` field. This is a default field you don't have to specify that exists everywhere, so you can use it to remove duplicate rows (which are identified here by duplicates/groups created with the fields `field1` and `field2`).

Useful references:

*   This approach [https://stackoverflow.com/questions/26769454/how-to-delete-duplicate-rows-without-unique-identifier](https://stackoverflow.com/questions/26769454/how-to-delete-duplicate-rows-without-unique-identifier)
*   Slightly alternative syntax at [https://stackoverflow.com/questions/6583916/delete-duplicate-records-in-postgresql/45606037#45606037](https://stackoverflow.com/questions/6583916/delete-duplicate-records-in-postgresql/45606037#45606037)
*   Further details at [https://www.postgresonline.com/journal/archives/22-Deleting-Duplicate-Records-in-a-Table.html](https://www.postgresonline.com/journal/archives/22-Deleting-Duplicate-Records-in-a-Table.html) for the `ctid`info.
