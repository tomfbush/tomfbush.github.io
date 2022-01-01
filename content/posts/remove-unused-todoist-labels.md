---
title: 'Todoist: Remove unused labels'
date: Sat, 24 Jan 2015 19:18:52 +0000
draft: false
tags: ['Development', 'python', 'todoist']
---

Want to remove your unused labels/tags from Todoist in bulk? The various GUIs will have you do this one at a time but I have written a small, not very efficient Python script that will do this for you. Here's how it works:

1.  You need to provide your API token (Which you can find in Todoist settings) in a file called token.txt
2.  Then download or copy the script from my [Todoist Remove Unused Tags GitHub repository](https://github.com/tomfbush/todoist-remove-unused-tags)
3.  Just run this using Python and it should work fine

Please bear in mind I've only tested this on my setup so it could go wrong, although it's highly unlikely. Pretty sure there isn't another way using Todoist to remove unused labels. Let me know how you get on in the comments. PS the code is awful, but works -- I plan to tidy it up in the future as I know for certain there are some unnecessary steps.