---
author: adam
date: '2007-09-06 23:17:05'
layout: post
slug: robocopy-microsofts-little-gem
status: publish
title: Robocopy - Microsoft's Little Gem
wordpress_id: '14'
categories:
- Tech
---

One of the things that has been hugely frustrating about my move to Vista is
that the backup tool is "dumbed down".  It only copies files it wants to copy
and it requires that you backup C: whether you want to or not.  All I wanted
to do was schedule a daily backup from my data drive D: to my archive drive V:
- I want any type of file copied...just a basic mirror type copy.  Apparently
this is impossible in the standard windows backup application.  Enter Robocopy
- a small command-line utility from Microsoft (included in Vista) that does
exactly this.  Robocopy can take a source and destination and perform a mirror
copy without a problem - and since it's a command-line application, you can
schedule it to run whenever you'd like.  It has tons of options to exclude
certain files/directories based on name, attribute, date, etc - but the basic
command to do a mirror copy is just this:

`robocopy d:\ v:\ /MIR`

Nifty huh?

