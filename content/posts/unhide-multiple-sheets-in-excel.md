---
title: 'Unhide Multiple Sheets in Excel'
date: Sun, 13 Jan 2013 10:13:40 +0000
draft: false
tags: ['excel', 'Software']
---

I recently had a need to unhide multiple sheets in Excel (maybe you call them tabs). Whoever sent me the original file had decided to spread their data out over so many extra sheets that it would have taken almost literally minutes to unhide them all. Naturally, I wasted even more time looking for a way to automate this process. I found two pretty good ways to unhide multiple Excel tabs.

Unhide Multiple Excel Sheets Using Custom Views
-----------------------------------------------

Okay, this one doesn't require any code and is EASY. It comes from [http://www.accountingweb.com/article/hide-and-unhide-multiple-excel-worksheets-ease/220551](http://www.accountingweb.com/article/hide-and-unhide-multiple-excel-worksheets-ease/220551) and works like this:

1.  Make sure all tabs are visible.
2.  On the View tab/menu, click on Custom Views.
3.  Add one and call it "Show All Worksheets" or similar.
4.  Make sure to tick the box that mentions hidden settings and press OK.

You can use the reverse of the above to hide the data sheets again by hiding them first and saving the view as "No data" or something. The only trouble with this method of revealing all your hidden Excel tabs is that it needs to be repeated for each new file. The following method can help with this.

Macro to Unhide Multiple Excel Sheets
-------------------------------------

This is a bit cooler but a bit more technical.

1.  Head over to [http://excel.tips.net/T002603\_Unhiding\_Multiple\_Worksheets.html](http://excel.tips.net/T002603_Unhiding_Multiple_Worksheets.html) for this one. There are two macros there, the first unhides _all_ worksheets. The second allows you to choose which to unhide
2.  To add this to a new macro, go to the Developer tab, then Macros, then create a new one. Make sure to create it in your Personal.xlsb so that it's universally available.
3.  Paste the code in and assign a keyboard shortcut (and/or add it to the ribbon).

There you go. I haven't gone into too much detail here because both the sites linked above are great, I just thought I'd summarise the two methods of unhiding sheets together. I seem to recall an Excel plugin that would unhide multiple sheets in Excel -- this was even easier than the above -- but I can't for the life of me remember the name, other than I think it was something like "Brian's Excel Tab Unhider", but I can't find that through Google. It'd be great if someone could point it out to me again... Choose Custom Views on the View tab or menu.Click Add, and then type a name for your custom view, such as All Sheets, and then click OK. Next, hide any worksheets as needed and then create a second view titled Presentation View, or a name of your choosing.
---
### Comments:
#### 
[Tobi @ Excel Formula](http://www.excelformulaslist.com "tobi.hossner@gmail.com") - <time datetime="2013-03-19 14:30:27">Mar 2, 2013</time>

Tom, you did the homework for me! I just recieved dozen files from client each had tons hidden sheets. Quick google search and whoala. Problem solved. Thank you!
<hr />
#### 
[Tom](http://www.tombush.co.uk "tomfbush@gmail.com") - <time datetime="2013-03-19 18:43:49">Mar 2, 2013</time>

Hi Tobi, glad I could help :) Nice site by the way, Excel is pretty much the only tool I use at work so I've already found a few ways to save time/make life easier. Thanks!
<hr />
#### 
[Tobi]( "tobi.hossner@gmail.com") - <time datetime="2013-03-19 23:26:51">Mar 2, 2013</time>

I can't live without Excel :) so sad, isn't it? Thank you, I haven't gone through many other articles of yours yet, but I surely will. Quick scan through told me there are a lot I could learn from you.
<hr />
#### 
[Tom](http://www.tombush.co.uk "tomfbush@gmail.com") - <time datetime="2013-03-20 13:51:23">Mar 3, 2013</time>

Haha, not sure I have much to teach but kind of you anyway :-) take care
<hr />
#### 
[WordPress Interview Questions](https://www.htmlkick.com/wordpress/wordpress-interview-questions/ "raymonddejesus230@gmail.com") - <time datetime="2021-03-29 13:17:09">Mar 1, 2021</time>

WordPress interview questions WordPress is a free and open-source content management system based on PHP & MySQL. Features include a plugin architecture and a template system. It is most associated with blogging but supports other types of web content including more traditional mailing lists and forums, media galleries, and online stores.
<hr />
