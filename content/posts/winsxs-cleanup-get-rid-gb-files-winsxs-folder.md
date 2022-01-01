---
title: 'WinSXS cleanup: how to remove GB of files in the WinSXS folder'
date: Sat, 01 Feb 2014 22:18:05 +0000
draft: false
tags: ['cleanup', 'Quick Tips', 'Windows 7', 'WinSXS']
---

This post is a quick one on WinSXS cleanup, and it works (for me). None of the instructions I found online helped me, including the KB2852386 fix on Windows update. Try this:

*   Go to C:\\Windows\\system32
*   Right click on cleanmgr.exe and Run As Administrator
*   Now, the relevant "Windows Update Cleanup" option and another for cleaning up Service Pack backups should appear. Tick them both
*   Proceed!

For me this worked a treat for WinSXS cleanup.