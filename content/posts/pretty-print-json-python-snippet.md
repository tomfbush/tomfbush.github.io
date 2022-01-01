---
title: 'Pretty print JSON in Python (snippet)'
date: Sun, 25 Jan 2015 09:52:03 +0000
draft: false
tags: ['Development', 'json', 'python']
thumbnail: "http://www.tombush.co.uk/wp-content/uploads/2015/01/json-300x300.jpg"
---

The below depends on the `json` Python module to 'pretty print' JSON output in Python. I found this useful when trying to write my [script to remove unused Todoist labels](http://www.tombush.co.uk/development/remove-unused-todoist-labels/ "Todoist: Remove unused labels").

```
import json # This function saves time printing JSON nicely
def pj(str):
   print(json.dumps(json.loads(str.content), indent=4))
   return pj(thing_containing_raw_json_here)
```

Note that in my case this was contingent on having used the `requests` module in the following fashion to already make sure the format is a bit jsonified, if I understand the `.json` at the end, which is not 100% guaranteed. `r = requests.post(todoistURL+"/login", params=loginParams).json()` There are numerous other ways to get JSON from an API or whatever than just using requests (I think people also use urllib?), but this is the route I took.


---
### Comments:
#### 
[Jake Coltman]( "jakecoltman@sky.com") - <time datetime="2015-12-14 16:05:31">Dec 1, 2015</time>

Nice article :), but some thoughts: - Generally bad practice to override built in language names (looking at you str) - The var name is called str but isn't a string as I read it, otherwise you wouldn't be calling str.content. Stand to be correct though! Can't json.dumps(json.loads(str.content), indent=4) become json.dumps(str,indent=4) ?
<hr />
#### 
[Tom Bush](http://www.tombush.co.uk "tomfbush@gmail.com") - <time datetime="2015-12-30 18:52:29">Dec 3, 2015</time>

Cheers Jake :) more than happy for you to impart your wisdom on stuff I post here :P
<hr />
