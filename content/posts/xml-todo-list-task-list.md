---
title: 'XML Schema for Todo/Task lists?'
date: Fri, 11 Jun 2010 19:02:16 +0000
draft: false
tags: ['Development', 'Productivity']
---

\[Edit: added a question mark to the end of the post title, in case anyone thinks I've written something formal... ideally someone else will because I don't have anything like the know-how :-) \] Okay, forgive me if I've got that terminology all wrong, but in practical terms I'm out of my depth here. I'm probably going over very old ground, but has anyone come up with an XML open standard/schema for declaring items on a task list or todo list (or multiple lists)? With all my indecision about which project management system to go with, and thinking about APIs and switching from Basecamp to TeamworkPM, and on a more personal level being stuck between Remember the Milk and Toodledo (and plain old text files), it would be really handy if I could take all my tasks with me and rely on all these different systems to supply the interface I need. I don't much care what methods they use to store my data, because I don't see that side. Basecamp for example (at the moment) doesn't have a way to show what my time estimate for a task is, or what tags I have associated with it, but there's no need for that data to be lost just because it's not supported by a particular interface. We're only talking a one-off import and then it can choose to preserve but not process extra information (until my one-off export into another task manager). I realise that BC is not just a task management app, there are writeboards and milestones and messages etc., and that XML files with loads of extra nodes or whatever might become unwieldy... but I'm sure there must be a way to unite the backends of all these systems for ease of transferring data... or maybe that's not what they want :-p ... As a basis for a format, I'd need the following at least, even if each task or system doesn't require or use them:

*   task (name)
*   project name (or top-level goal)
*   list name
*   completion status (boolean would be fine but different interfaces could interpret anything less than 1 as incomplete)
*   due date
*   priority

but there could also be

*   start date
*   responsible party
*   notes
*   "tags"
*   status (à la Toodledo)
*   etc.

I just find it frustrating that I can take code/graphics/audio files/whatever with me quite easily between different programs as their features and interfaces change and better each other... but it's not so easy with the most vital day-to-day item, the list of tasks itself! I suppose that would be a strong vote for the TODO.txt system -- not being tied down to an interface per se. But as much as I like TODO.txt, it hasn't been taken up as a standard (perhaps it should have been) by the web. I think that's what I'm trying to get at, a way that the web might go for... SET MY TASKS FREE! :-P
---
### Comments:
#### 
[Jay](http://www.kilobitspersecond.com/ "topdownjimmy@gmail.com") - <time datetime="2011-06-20 15:46:09">Jun 1, 2011</time>

I'm surprised there aren't more people demanding this (at least seemingly so, given the limited search results I got from Google). I think it would be smart to find out which task managers already export as XML, and to study their schemata. An ideal universal solution would resemble existing formats so that applications that already have an XML schema won't have to change much. Other than the example at [old\_roy](http://www.tombush.co.uk/productivity/xml-todo-list-task-list/#comment-79)'s link, which is way too minimal, I don't think I've ever even seen an attempt at this. I have a feeling that if someone were to try to define a task list XML schema, a lot of smarter people would come out of the woodwork to tell them where they've gone wrong, and we might actually end up with something robust, expandable, and relatively future-proof that people can agree upon.
<hr />
#### 
[old_roy]( "roy.tscorp@gmail.com") - <time datetime="2011-02-11 22:38:11">Feb 5, 2011</time>

Also - Kplato for linux kde distros will export an entire project as xml including task lists.
<hr />
#### 
[Tom]( "tomfbush@gmail.com") - <time datetime="2011-06-20 20:47:03">Jun 1, 2011</time>

Jay, thanks for the input. I just might be tempted to be the "someone" in your suggestion, so that smarter people might come out of the woodwork ;-) Totally agree that the way to go is to look at what is in use already, no matter how quirky or software-specific. Leave this with me, I may set up a wiki or similar to help progress this. Cheers Tom
<hr />
#### 
[old_roy]( "roy.tscorp@gmail.com") - <time datetime="2011-02-11 21:41:39">Feb 5, 2011</time>

Interested in the same thing.....check this link..... http://willcode4beer.com/design.jsp?set=todoList This might give you a start....
<hr />
#### 
[Tom]( "tomfbush@gmail.com") - <time datetime="2010-11-02 20:10:54">Nov 2, 2010</time>

Hi Trever -- no I didn't... if there was one in wide usage I suppose there's a chance it might be listed here: http://en.wikipedia.org/wiki/List\_of\_XML\_schemas What sort of use cases were you thinking of?
<hr />
#### 
[Trever Shick]( "trevershick@yahoo.com") - <time datetime="2010-10-29 14:22:36">Oct 5, 2010</time>

Did you ever figure this out? I'd like a common model as well for tasks so i'm googling today.
<hr />
#### 
[osimod](http://egov20.wordpress.com "david.osimo@gmail.com") - <time datetime="2012-06-18 08:08:51">Jun 1, 2012</time>

Came across the post while searching for such a solution. I also feel the need for this. We need a microformat for task just as .ics for calendars. So that people can send around email with task attached (just as for ical events) which are directly imported into everyone's task manager. any update?
<hr />
#### 
[Tom]( "tomfbush@gmail.com") - <time datetime="2012-06-20 06:43:16">Jun 3, 2012</time>

Hi there -- I was beginning to make some notes at http://wiki.tombush.co.uk/index.php?title=XML\_for\_task\_management however this morning I found the following: http://microformats.org/wiki/task -- it needs updating but this looks like what we're after. Take a look and let me know, feel free to add to the wiki I set up if it's of any use. Best Tom
<hr />
#### 
[The missing standard for todo apps | Feelmaking](http://www.feelmaking.it/2012/07/the-missing-standard-for-todo-apps/ "") - <time datetime="2012-07-04 10:56:02">Jul 3, 2012</time>

\[...\] the core concept. I also discovered that Tom Bush (and probably a lot of other folks) had the same idea in 2010, but today there’s still no real progress, so I decided to publish this post anyway \[...\]
<hr />
#### 
[Dex]( "dex@pirho.net") - <time datetime="2020-04-26 09:19:50">Apr 0, 2020</time>

The iCalendar format (RFC 5545) has a VTODO feature and this is also available in the xCal format (RFC 6321).
<hr />
#### 
[Matthew Harwood Leach]( "matthewhleach@ge.com") - <time datetime="2015-06-13 00:20:49">Jun 6, 2015</time>

I believe you were on to something with the XML tag philosophy regarding To-Do list. I would even expand that to any note you take, regardless of subject. Things you want to remember, etc. but want the means (or future means) to integrate and actually use/remember/analyze the data. Maybe we haven't quite defined the problem or the solution, but I've done some work in this area and would like to re-open the case. Feel free to email me at matthewhleach@gmail.com if the author or comment authors would like to continue to sharing notes. Thanks, Matt
<hr />
#### 
[Tom Bush](http://www.tombush.co.uk "tomfbush@gmail.com") - <time datetime="2015-06-13 02:36:33">Jun 6, 2015</time>

Hi Matt Will drop you a note in the coming days. The abundance of todo or note taking apps available definitely makes some transferable schema appealing, and would put the pressure on them to make their interfaces the selling point whilst we own our data. Thanks for getting in touch! Tom
<hr />
