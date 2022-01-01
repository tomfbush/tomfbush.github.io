---
title: 'Windows Update: Same Updates Over And Over Again (FIX)'
date: Mon, 25 Jun 2012 20:25:58 +0000
draft: false
tags: ['fixes', 'Software', 'vista', 'windows']
---

\[caption id="attachment\_250" align="alignright" width="199"\][![If Windows Update Failed One More Time My Laptop Would Look Like This](http://www.tombush.co.uk/wp-content/uploads/2012/06/smashed-199x300.jpg "If Windows Update Failed One More Time My Laptop Would Look Like This")](http://www.tombush.co.uk/software/windows-update-same-updates-over-and-over-again-fix/attachment/smashed/) If Windows Update Failed One More Time My Laptop Would Look Like This (I Don't Know Who That Girl Is Though)\[/caption\] There was me thinking that the Windows Update mechanism was designed to streamline updates to the operating system, eliminating the need to go to a website to download fixes and patches. Ha ha ha. Without realising it, I've been repeatedly shutting down to install the same Windows Updates on Vista for the past 2 weeks. Windows Update never registered the installs and kept on asking me to do it again. Many of the help sites I found just suggested ignoring the updates in the future, which didn't seem sensible given that they were mostly security updates, i.e. important, and one optional update that supposedly was for some hardware I had just bought. The answer lay here: http://support.microsoft.com/kb/910339 There is a downloadable fix offered by the Microsoft website (a "Fix It" troubleshooter) that seems to have done the trick. I followed the steps and it identified that there was a problem with Windows Update, and reset its database. Happy days, now I can actually shut down the computer at a normal speed instead of it taking half an hour to install the updates _again_. So, in summary:

1.  Go to  http://support.microsoft.com/kb/910339
2.  Download and run the Fix It program (if it doesn't pop up, look for it on the page, it's there)
3.  Run it, follow the prompts; it only gave me one option so it didn't matter if I picked auto or manual fix
4.  Try to install the updates that keep on appearing
5.  Hopefully now you're done (you might need to restart too)

Hope that works!
---
### Comments:
#### 
[Tom]( "tomfbush@gmail.com") - <time datetime="2012-07-30 20:32:17">Jul 1, 2012</time>

Hi Dee! Thanks for the comment. I always thought that I would miss all my Windows games if I moved to Mac. As it happens, I don't have time to play them any more so it wouldn't have been a problem! What did you go for out of interest? Is there a reason to choose a desktop over a laptop Mac beyond the usual pros and cons of laptop/desktop? I know that OSX is a form of Linux, which in my experience with Ubuntu and Fedora was much smoother with updates than Windows. Is this still the case? Cheers Tom
<hr />
#### 
[Dee Ankary](http://moonpreneur.net "dee.ankary@gmail.com") - <time datetime="2012-07-30 18:12:24">Jul 1, 2012</time>

Hi Tom, Great that you posted this easy-to-follow set of instructions for getting around this problem. I discovered the Fix It tool with Windows 7 on our home computer, and it does help on most occasions. Probably not what you want to hear, but I ended up making the switch to Mac around 18 months ago, and never looked back. I still run Windows on my Mac under VM Fusion though ... Cool blog btw. Dee
<hr />
