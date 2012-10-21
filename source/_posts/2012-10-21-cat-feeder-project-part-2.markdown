---
layout: post
title: "Cat Feeder Project - Part 2"
date: 2012-10-21 14:47
comments: true
categories: [projects, catfeeder]
---

I spent some time this weekend working on the hardware to provide cooling for the cat feeder.  The goal is to get the cat feeder to the same temperatures as a refridgerator.  I want to keep the unit as trouble free and cost effective as possible, so I don't want to go the compressor route.  The option I'm prototyping is using a [thermoelectric cooling (TEC)](http://en.wikipedia.org/wiki/Thermoelectric_cooling) chip (known as a Peltier element).  If you apply power to a TEC, it will cool on one side and heat on another.  If you're trying to cool, you have to remove the heat from the hot side of the TEC with an external heatsink.  TECs are very inefficient, but they should be able to do exactly what I need for this project.

##The Prototype Setup
[![](http://share.adambyram.com/2012-10-21-cat-feeder-project-part-2/Cooling-Test.jpg)](http://share.adambyram.com/2012-10-21-cat-feeder-project-part-2/Cooling-Test.jpg)

###Components

- [Arduino Uno R3](https://www.adafruit.com/products/50)
- [Adafruit Adjustable Breadboard Power Supply](https://www.adafruit.com/products/184)
- [12V 1A Regulated Power Adapter](https://www.adafruit.com/products/798)
- [2 x N-Channel MOSFET 60V 30A](https://www.sparkfun.com/products/10213)
- [70mm Heatsink and Fan](https://www.sparkfun.com/products/10686)
- [40mm x 40mm Peltier element](https://www.sparkfun.com/products/10080)
- Breadboards, jumper wires, heatsink compound, and a few push buttons

###Assembly

I used a few push buttons on the breadboard next the to Arduino so I could control the power to the heatsink's fan and the TEC.  The Arudino's PWM output is sent to the two MOSFETs which varies the amount of current sent to the fan & TEC.  The fan & TEC are both connected to the 12V 1A regulated power supply via the Adafruit breadboard power supply.  I originally tried to run the TEC at a lower voltage than 12V by using the adjustable power supply, but it turned out to be easier to just hook both items directly to the 12V supply.

###Results

The power supply can't provide enough power to run the TEC with the MOSFET wide open.  One the TEC starts drawing a reasonable amount of power, the fan starts slowing down and evetually, the TEC will draw so much current that everything else shuts down.  I was able to run the fan with the MOSFET wide open and the TEC MOSFET set to about 67% power.  At those settings, the fan runs (at less than full speed) and the TEC is able to cool quite reasonably.  The TEC MOSFET started getting quite hot, so I added a passive heatsink on there.

The at the end of the day, I was able to use the settings above to take the TEC from 75F down to 38F in just a few seconds.  I ran the whole setup in this configuration for about 5 minutes with no issues.  Overall, I'm very happy to get near freezing temperatures with the relatively small power supply.

###Next Steps

I want to get a bigger power supply.  I'd really like to get an adjustable lab power supply so I could try different amounts of current to see what exactly I need, but I'm thinking I'll try a 12V 2A power supply.  I need to see how much current I can run through the jumper wires if I upgrade the power.  The current test didn't get the wires hot, but I'm not sure how much more current they'll take.

At this point, I just need to get the TEC a little cooler while getting the fan to run faster on the heatsink.  I'm not too worried about the hinksink though...it never got that hot even with the fan running slower.  I'd like to build a small enclosure so I can experiment with cooling air and not just the surface of the TEC.  This will probably mean I end up building a styrofoam box (or buying one) and mounting a heatsink & fan on the cold side of the TEC to distribute the cooling power. 