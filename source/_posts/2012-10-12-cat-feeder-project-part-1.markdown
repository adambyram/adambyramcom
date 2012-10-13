---
layout: post
title: "Cat Feeder Project - Part 1"
date: 2012-10-12 23:29
comments: true
categories: [projects, catfeeder]
---

Some of you may know my cat situation.  If you're not aware, the long and the short of it is that my cats used to only eat dry cat food.  One of the cats ended up getting very sick when I moved to Los Angeles.  After she recovered (she's fine now), she decided she'll never eat dry food again and only eats very specific wet cat food.  

The problem is that I have two very nice automated dry food feeders that I can't use.  Both cats need to be on a schedule to help control their weight.  So I started researching wet cat food feeders and it turns out, there aren't many.  Not only that, the feeders that are out there all use ice packs which limit you to 8 or maybe 12 hours of feeding.  That's totally not acceptable to me so I've decided I'm going to try to design my own wet cat food feeder.

### What

So what is this thing?  Well, it's a small (~2 ft wide) unit that has a certain number of rotating food cups.  The food cups can be filled with wet food (or dry food) and the unit can be programmed to expose each food cup to the cats on a specific schedule.  The unexposed food will stay seal up inside the unit and a cooling unit will keep the unexposed food nice and cool.

The goal is to have the unit keep food at refridgerated temperatures (TBD what that means) consistently to allow food to be stored in the unit for up to three days.  That seems to be the maximum time wet food is allowed to be refridgerated based on manufacturer information, so that'll be the target for version 1.  

If the machine can feed twice a day for an overnight trip or once a day for a long weekend trip, it'll be fantastic, so that's the target.

### Why

On top of the issues mentioned above, I really want a exposure to the hardware + software world.  I've worked on software for quite a long time and basically everything I've built is totally virtual in nature.  That's all fine and good, but I'm really wanting build something physical.  Of course, some software will still be needed, but I'll also get some electrical engineering, product design, and CAD modeling.

The other part of the why is that I really want to be able to go on a long weekend trip and not have to worry about the cats getting fed.  Today, we basically can't be gone for longer than about 8 hours at a time without having someone come by to feed the cats.

### How

I'm planning on building everything with some pretty common parts.  The initial design / prototype is going to be all plastic, mainly because I'm getting a [3D printer](http://www.kickstarter.com/projects/2105227104/ultra-bot-3d-printer) in December.  The general electronics won't be anything super special.  For the prototype, I'll be using an Arduino Uno for overall control, a motor controller board to rotate the food dish, a external power module to power the cooling system, and a few other random bits.

For cooling, I'm planning on using a Peltier cooler.  They aren't very efficient, but they are relatively easy to use and they can work reasonably well (based on my experience with a little mini fridge).  They are also pretty cheap, so it's quite cost effective from a component perspective.  The cooling will be the trickiest aspect of the whole project.

### When

Well, I've already started playing with the basic components and working on the hardware design (the body of the feeder, not the electronic components).  The 3D printer won't be available until later in December, so I can't start working on the real prototype until then, but I'll be able to play with the cooling system this month and into November.  My goal is to have a really rough 3D model ready by the time the printer is available.  I'm assuming I'll needed lots of revisions to the plastic parts since all of this (the design process, printing process, and design software) is new to me, but I want to be able to hit the ground running.

As far as the finished product, I'm hoping to have a totally working prototype in Q1 2013.  Will that happen? I have no idea, but I really, really want this product so I'd like to have something working sooner rather than later.

### What's Next

I plan to blog my progress on this project.  It's as much for me to keep track of things as it is for everyone else to follow along.  Next time, I'll show the current stage of the design and share some thoughts on the design process as well as the design software I'm using.  This should be a fun project, so I hope you have as much fun following along as I'm having building this thing.