---
title: 'Easy Sumif in R Using The Aggregate Function'
date: Fri, 24 Apr 2015 20:47:08 +0000
draft: false
tags: ['aggregate', 'R', 'sumif', 'excel']
categories: ['analytics']
thumbnail: "https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/R_logo.svg/2560px-R_logo.svg.png"
aliases:
  - /r/sumif-in-r-like-excel-aggregate/
---

This is a really simple (i.e. probably even the most basic possible) example of using the built in aggregate() function in R, basically a sumif in R. Given a set of data where column a is the values and column b contains the data by which you wish to group (in this example categorical data with values of a or b):

```
> data
    a b
  1 0 a
  2 0 a
  3 1 b
  4 2 a
  5 2 b
  6 2 a
  7 3 b
  8 4 b
  9 7 b
```

The aggregate function as I have used it below takes the following arguments -- data$a is the column we are applying a function to; by = refers to a list of names and references to aggregate things by (in this case just one column, so the list has a single element); finally the function we are using here is the built in sum (but this could be a function of your own making, or a mean, or whatever):

```
> aggregate(data$a, by = list(Category = data$b), FUN = sum)
   Category x
 1 a        4
 2 b        17
```

That's it. This replaces the most basic Excel sumif functionality using R's aggregate function.

