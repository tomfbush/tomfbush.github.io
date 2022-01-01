---
title: 'A Bit Better RTM tweak - hide empty lists in Remember the Milk'
date: Sat, 14 Nov 2009 16:37:58 +0000
draft: false
tags: ['greasemonkey', 'Productivity', 'remember the milk']
---

I use [Remember the Milk](http://www.rememberthemilk.com/ "Remember the Milk") to keep track of the following:

*   "project-less" tasks that do not require a structure around them
*   tasks that repeat (not one of the strong points of Basecamp et al)
*   tasks that need to be worked on at more specific times

For personal, non-collaborative tasks, I think RTM is pretty clever. There's no respite though. It gives you quick access to empty lists so you can add things to them easily. This stresses me out. I'm the kind of person that likes it when Basecamp shows me this:

\[caption id="attachment\_48" align="alignnone" width="300" caption="I am not responsible"\][![I am not responsible](http://www.tombush.co.uk/wp-content/uploads/2009/11/i-am-not-responsible-300x99.jpg "I am not responsible")](http://www.tombush.co.uk/wp-content/uploads/2009/11/i-am-not-responsible.jpg)\[/caption\]

The point is, it's nice to use an interface that understands the intense, forboding pressure you are under, and knows when to hold back and tell you there is nothing to do.

**A Bit Better RTM**, which cleans up Remember the Milk and moves the lists into a sidebar to the left (amongst other things) started out as a [Greasemonkey script](http://userscripts.org/scripts/show/32518 "A Bit Better RTM script"), although now there is a [Firefox extension](https://addons.mozilla.org/en-US/firefox/addon/14832/ "A Bit Better RTM firefox extension") too.

I don't know when I first started using the script but I made a really minor tweak to it that automatically hides empty lists in Remember the Milk which gives me a feeling of success as the, er, list of lists gets smaller. **I don't want to be reminded of all the projects that I have on my plate**, especially if there is nothing I need to do to them right now. (If you need to see those empty lists, change the code so that instead of being hidden, the empty lists are grayed out/in a small font/struck through).

The key is this part of code:

```
if (tasksCount > 0)
 listItems\[i\].firstChild.innerHTML = listItems\[i\].firstChild.innerHTML + " (" + tasksCount + ")";

 else
 {
 listItems\[i\].style.display = "none";
 }
```

You can install the script from here:

**[Hide empty lists in Remember the Milk](http://userscripts.org/scripts/show/61989 "Hide empty lists in Remember the Milk")**

I'm pretty sure the original script has now changed a lot, but the one I use still appears to work with RTM so that's fine with me. Also, I have to confess, I don't know what happens if there are no incomplete items in any lists, I suspect it looks quite bad.