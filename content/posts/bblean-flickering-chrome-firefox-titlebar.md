---
title: 'bbLean flickering with Chrome/Firefox/other: FIX'
date: Sat, 01 Feb 2014 21:09:02 +0000
draft: false
tags: ['bbLean', 'fixes', 'Google Chrome', 'Software']
---

I just loaded up bbLean as a way of speeding up my old Win7 laptop, only to discover that Google Chrome (the app I use the most) was flickering really badly because it has its own skin, and bbLean was trying to apply its own titlebar too. I would have just commented on Nimret's blog to say thanks, but it seems that comments are turned off. I decided to post thanks and the method here instead (but you can read the original [here](http://www.nimret.org/2011/03/30/1301529780000.html)). The answer to Chrome flickering with bbLean is:

1.  Open the blackbox right click menu from the desktop
2.  Go to _bbleanskin_ then _Edit Exclusions_
3.  Type 'chrome.exe' at the end of the file

This should work for any applications facing the same problem. \[caption id="attachment\_421" align="alignnone" width="338"\]![bbLean flickering fix](http://www.tombush.co.uk/wp-content/uploads/2014/02/bbLean-flickering-fix.png) Go here to stop bbLean flickering with Chrome and other apps\[/caption\] Let me know if this doesn't fix your bbLean flickering issues. Edit: This reportedly affects other apps with a bespoke title bar such as Firefox
---
### Comments:
#### 
[Metaphor]( "nemesis@funny.cat") - <time datetime="2014-05-21 23:16:09">May 3, 2014</time>

For Firefox: Go to Menu —> Customize Look down in the bottom left corner, click "Title Bar" (you want the button to look pushed). That's all. Enjoy.
<hr />
#### 
[Tom](http://www.tombush.co.uk "tomfbush@gmail.com") - <time datetime="2014-05-25 10:02:41">May 0, 2014</time>

Thanks Metaphor :)
<hr />
#### 
[Guy]( "presidentlordjoe@gmail.com") - <time datetime="2014-10-27 02:58:04">Oct 1, 2014</time>

It's still not working for me with Microsoft office 2013 (all the programs involved). The program name for, say, Word 2013 is "winword.exe", and even when I type it into the exclusions list, it still has the flickering title bar. Chrome and Firefox worked just fine for me, it's just office
<hr />
