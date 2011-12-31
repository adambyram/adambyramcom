---
author: adam
date: '2009-10-28 13:01:25'
layout: post
slug: my-att-u-verse-experience-in-knoxville
status: publish
comments: true
title: My AT&T U-verse Experience in Knoxville
wordpress_id: '77'
categories:
- Tech
---

I've had quite a few people ask about my recent AT&T U-verse install, so I
thought a quick blog post was in order. Keep in mind, my install happened
during the first week of the Knoxville, TN U-verse rollout - so I'm sure
things will go faster (as far as the installation goes) as they do more and
more installs in this area.

I chose to go with U-verse because I live in an older neighborhood in
Knoxville and my high speed internet choices are fairly limited. I've had
3Mbps DSL from AT&T for the last 3 years and it's been decent, but I really
needed more upload speed. I'm a software developer so I usually have lots of
large software updates I need to download quite often and I frequently have
fairly large chunks of data I need to upload to a server on a regular basis
(Dropbox, Subversion, etc.). I ended up going with AT&T U-verse since they
offer a package with 18Mbps download and 2Mbps upload...this was my main
consideration for choosing U-verse, not the VoIP service nor the TV service. I
want to make it clear that I didn't compare the TV and phone services to other
providers...so if that is your main focus, this writeup may not be useful to
you.

**Speed Test - Before & After** _All tests were performed with www.speedtest.net on a MacBook running Snow Leopard connected to my wireless LAN - this is my most common usage scenario, so it's what I decided to test with.  Also, ignore the "distance" in these speed tests...all were performed in Knoxville at the same location._  

Before U-verse - Speed Test

[![](http://share.adambyram.com/2009-10-28-my-att-u-verse-experience-in-knoxville/SpeedTest-DSL.png)](http://share.adambyram.com/2009-10-28-my-att-u-verse-experience-in-knoxville/SpeedTest-DSL.png)

After U-verse - Speed Test

[![](http://share.adambyram.com/2009-10-28-my-att-u-verse-experience-in-knoxville/SpeedTest-Uverse.png)](http://share.adambyram.com/2009-10-28-my-att-u-verse-experience-in-knoxville/SpeedTest-Uverse.png)

From this quick test, you can see my download rate is much higher, but my
upload rate also got a massive improvement.  The ping time got cut in half as
well - so it's a win-win-win with the U-verse upgrade.  The thing is, the
download rate isn't anywhere near the max rate of 18Mbps, so I decided to try
a speed test against the Atlanta, GA data center since I would assume they
have more capacity than Morristown...

Speed Test - Atlanta

[![](http://share.adambyram.com/2009-10-28-my-att-u-verse-experience-in-knoxville/SpeedTest-Uverse2.png)](http://share.adambyram.com/2009-10-28-my-att-u-verse-experience-in-knoxville/SpeedTest-Uverse2.png)

Nice huh?  That's quite close to the max download rate and a very respectable
upload speed...and the ping is lower still.  So the bottom line is U-verse
blows regular DSL out of the water and it is generally better than cable or at
least very comparable.  One of the things I don't like about cable internet is
they use different methods to boost your speeds for short periods of time.  So
you may have a 12Mbps package and for 30 secs - 2 minutes, you may get that
speed when starting a download, but if you're downloading something large, you
will usually notice your download speed dialing back pretty
drastically...whereas I should (in theory) have these U-verse speeds
throughout the whole download.  Realistically though, you're going to be very
unlikely to find a single server that can provide you with a download at these
rates, so the only way you would be able to get this much data flowing would
be to have quite a few downloads going on simultaneously.

**The Installation**  
Now that the speed test is out of the way, you may want to know about the
installation process.  When I signed up for the install, I was told the
install takes between 4 to 6 hours depending on the services I wanted
installed and the specifics of my house/neighborhood.  The U-verse install
requires two different groups - one is an external group that hooks up your
new equipment on the outside of your house and the other group does everything
inside the house.  In my case, I heard from both groups at 9am - both called
to confirm the appointment and to let me know they were on the way.  The
external guy got here around 9:30am and he started checking the lines outside
my house.  The internal guys got here around 9:45am and I gave them a quick
tour of the places I wanted U-verse.  The external guy worked until 11 or a
little after getting everything prepped and getting some electronics added on
to my house that connect back up to the utility pole.  While he was doing
that, the internal guys explored the attic and crawlspace to determine the
best way to run my new wires.

I have an older house and even though I did have coax cables in most of the
rooms, the cables were always on the opposite wall from my TVs (I have not had
cable for over 3 years...so placement in relation to the cables wasn't exactly
important prior to today).  After talking to the U-verse guys about this, they
agreed they should go ahead and run new wires to all of my TVs...but here's
the awesome part: they ran Cat 5e cables to all my rooms *for free* instead of
coax!  That was a HUGE win for me...why?  Because now I can add a network
switch in any room with one of the new network jacks and I've got a way to
hardwire in my other goodies...specifically, my Xbox 360 and my Blu-ray
players.  If you already had coax cable that was close to your TVs, I don't
think they would run anything for you since they prefer to use existing
wiring.  Even if they do run new stuff for your install, *you* must ask for
Cat 5e instead of coax if that is what you want.  They can install either one
usually unless there are specific environmental conditions at your location -
in which case they may not give you a choice.  Anyway, it took them maybe an
hour to hour and a half to run the network drops (I had four sets total in my
case...all from the crawlspace).

By this time, the outside stuff was done and tested.  Both teams must test the
line once it's ready to go - until that point, you don't really know whether
you can actually get U-verse service or not.  If you can't, I don't know what
happens...in my case, both teams agreed that I had an excellent signal here so
we could proceed with installation of the Residential Gateway (the "RG").  So,
they finished up all of the network jacks (adding faceplates, etc.) and then
connected up the RG and the backup battery (a small Belkin UPS...keeps the net
and VoIP up for 4 hours if the power goes out).  The RG essentially *IS* the
U-verse service...it controls everything.  It has a router (wired and
wireless...b/g only), the VoIP system, and the TV connections.  So if this box
isn't happy, nothing is going to work.  It's important to note that this RG
box needs a true, three prong grounded electrical outlet...I have a 50 year
old home, but luckily a handful of my outlets were updated to be grounded just
before I bought this house.  If you're thinking about U-verse and you have an
older house, make sure you have one of these outlets or you won't be able to
install...you can't use an adapter for this part, you *must* have a real
grounded outlet near the RG.

As luck would have it, my RG was not happy.  No matter what they did, it just
wouldn't connect to the network.  The techs tried everything they could think
of, but after about 2 hours of troubleshooting it, they decided it we should
try another RG.  At this point, the installation was crossing the 7 hour mark
(the guys didn't even take a lunch break...).  This time, the RG connected
properly.  Even when the RG works, the initial setup still takes about 15
minutes while it configures itself.  Once that was done, I had to connect to
the RG from my MacBook and finish a few last steps on the AT&T website.  Once
all of that was out of the way, the techs connected up all of my TV boxes and
let them sync.  All of them had to perform an automatic update that took
another 10-15 minutes to complete.  Finally, we did a quick test of my phone
system, finished porting my number to the new system, and then they gave me a
quick tour of the U-verse software on the DVR.  It was 6:30pm and the
installation was completed.

**So, was it worth it?**  
I've had the service for less than a day as I write this, but I can say that
this was 110% worth it for my purposes.  Heck, just getting these great upload
and download rates makes it worth it for me, but getting my house wired with a
wired gigabit network was an unbelievable bonus.  Will I watch all 450+ TV
channels?  No, I'll probably watch 20 or less any given week.  If you like TV
though, this package has as much as any of them.  I don't use the landline
phone much, so I'm not sure how useful the VoIP upgrade will be...call quality
sounds much better (I had some noise prior to this upgrade), but I wanted to
keep my Knoxville number, so I kept the phone service for the moment.  I think
a typical install in a newer home that already had existing coax (or ethernet)
cable in all the right places would be much, much shorter than my
install...maybe 2-4 hours.  So if you're thinking about getting U-verse, don't
let the length of my install deter you - it's very unlikely it'll take longer
than 6 hours max.  All of the guys I dealt with during the install were a
pleasure to work with - other than the technical issues with the bad RG
hardware, everything went as smoothly as one would want.  The real question is
the long term support - will AT&T keep up the great customer service I
experienced or will they drop the ball now that I'm committed to U-verse?
Only time will tell, but I can certainly recommend U-verse at this point.

UPDATE (10/30/2009): It's been a couple of days now and I'm still very happy
with the service.  The only "issue" I've found is that I misunderstood the
stream limit with U-verse as far as TV programming.  I thought all boxes would
be able to watch any channel (HD or SD) and the DVR box could do 4 channels
(all recording or watching 1 and recording 3).  What I didn't realize was that
your entire U-verse system can only support 4 channels simultaneously and of
those 4, only 2 can be HD.  So if you have three boxes like I do, you can't
watch live HD content on all three boxes at the same time unless you're
watching the same show(s) on two or more of the boxes.  If you have lots of
TVs in your house, you may hit this issue pretty quickly.  In my case, I hit
the issue because three of the shows I like to watch come on at the same time
on the same day of the week...when I tried to set the DVR to record all of
them in HD, it told me I couldn't.  I can drop one of the shows down to SD and
it's fine, but while the recording is going on, I won't be able to watch any
other channels in HD (it gives you a blue screen and tells you no more HD
channels can be used until the recording has stopped).  For me, this isn't a
deal breaker, but I thought I should put a note on here since this limit
wasn't clear to me...I knew the limit of 4 streams on the DVR box, I just
didn't realize that was a limit on the whole U-verse install.

