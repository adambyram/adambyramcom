---
layout: post
title: "Switching to Octopress"
date: 2011-12-31 19:08
comments: true
categories: 
- Tech
---
I've been looking into Octopress for a month or so now and I finally decided to take the plunge.  As of now, this blog is now powered by Octopress (more or less out of the box) instead of WordPress.  I'd like to change the theme a bit, but it's good enough that I'll leave it for now.

### WordPress -> Octopress
Nothing was wrong with WordPress itself, but I just didn't use any of the features it offered.  I'd rather just type the blog posts in a regular editor instead of a textbox on a webpage.  There are some great tools out there that help with that of course, but I just don't need the features there either.  In addition, maintaining WordPress means logging in pretty often to check for updates, apply them, make sure the database is backed up, etc.  All of that would be just fine if I received enough benefit to offset the time there, but I just didn't.

### Enter Heroku
In addition to switching the blogging engine, I moved the physical blog from Linode over to Heroku + Amazon S3.  My blog is very low traffic, so I don't need a high powered VPS host that I have to maintain & patch.  Heroku offers a free account if you don't need much power and can live without a database (well, effectively without a DB - a 5MB one is included).  I decided to go ahead and put any post specific images/files onto S3 since Heroku offers a limited amount of local storage and I can also redeploy back to Linode if something doesn't work out at Heroku.  For the record though, I *love* Linode for a Linux VPS host.  I highly recommend them as long as you're comfortable dealing with Linux via the command line.

### Simplicity
As I get older, the technology side of things appeals to me less and less.  I still love technology in general, but the nitty gritty details of what platform/framework/OS/whatever is the best is less and less interesting to me.  I'm more interested in the best way to deliver a solution in a way that is as simple as possible.  That doesn't mean I'm adverse to complexity under the hood though. It means I value the experience, productivity, and the ability to simply get things done over the technical aspects of a solution.