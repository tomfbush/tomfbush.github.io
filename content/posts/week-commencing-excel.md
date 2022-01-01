---
title: 'Week Commencing Excel Formula'
date: Wed, 17 Dec 2014 20:11:45 +0000
draft: false
tags: ['Excel', 'formula', 'media', 'week commencing']
categories: ['analytics']
aliases:
  - /excel/week-commencing-excel/
---

A lot of the data we use is on a daily basis. This is great for more granular insight and for pacing media spend etc. Sometimes however you want to bundle it all up into nice, weekly buckets (often based on 'week commencing') so that you can look at how weeks affect the sales pattern over the month, for example. This might be harder to see based on daily data. If you need to calculate the week commencing date in Excel (i.e. the date of the Monday that another date falls in) then the following week commencing Excel formula is definitely your friend: `=B2-WEEKDAY(B2,3)` Let’s look at what this means. B2 is the cell that contains the date for which you want to calculate the "week commencing” date. As a date in Excel, this has a value (usually in 5 digits, starting with 4, in this day and age). WEEKDAY is a function that returns a number that represents the day of the week in the first argument (in this case our date in question, B2) based on a certain starting point (in this case, 3, which means ‘give Monday a value of 0 and increase that by 1 for each day of the week in order).

Putting it together to get the week commencing date
---------------------------------------------------

If it already is Monday (and you want to calculate the week commencing date based on weeks starting on Monday) the formula above says “the date returned by this formula should be equal to the date in B2 minus 0.” This is going to return the date already in B2, which is what we want, because it IS a Monday. If it were a Tuesday, it would say "the date in B2 mins 1", which would of course give us the week commencing date of the Monday we want. In this way it increases until minus 6 for the Sunday, and then goes back to 0 the following Monday.

Changing how Excel calculates the day of the week value
-------------------------------------------------------

If you don't want your formula to use Monday as the start of the week (or use 0 for the value) then you have these options instead of the 3, as the second argument of WEEKDAY() (straight from the Microsoft Excel help file):

> 1 or omitted returns numbers 1 (Sunday) through 7 (Saturday). Behaves like earlier versions of Excel. 2 returns numbers 1 (Monday) through 7 (Sunday). 3 returns numbers 0 (Monday) through 6 (Sunday).

I don't know of any other more efficient way to calculate week commencing in Excel.
