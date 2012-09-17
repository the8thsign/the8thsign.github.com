---
layout: post
title: 'Macbook Random Shutdowns'
tags:
  - apple
  - applecare
  - macbook
  - osx
  - random
  - reboots
  - vista

---

<img src="http://www.the8thsign.com/wp-content/uploads/2006/08/lifeisrandomsm.jpg" alt="Lifeisrandomsm" border="1" height="300" hspace="4" vspace="4" width="400" />

My Macbook has RSS, and I'm not talking about Really Simple Syndication. My 3 month old Macbook has recently started randomly rebooting itself. Random Shutdown Syndrome. It started 2 weeks ago, July 6th to exactly, out of no where. Outside of the discolored palm rests, the machine has been flawless.

For me it all started while I was installing Tiger on an external Firewire drive. Happened about 5-6 times that day, most of them in a row. I couldn't get the system to boot until i reset the PMU. Since then I was installing Vista pre-RC1 using Boot Camp and it rebooted on me during the install there too. I can be surfing the web, reading rss, listen to music, or nothing at all. All of a sudden, BOOM! black screen. Hit the power button then BOOM! black screen again. This goes on for 3 or 4 tries before it will boot up usually. Right now I'm getting about 5 shutdowns a week but last night alone i had 3; 2 while inside Windows Vista.

It happens for while using Vista, OS X on 2 different internal drives, OS X on an external firewire so its not the operation system or software. I've used two different hard drives and two different set of memory chips. Does not matter. I did not have the problem prior to 10.4.7 but the update has nothing to do with it. The <a href="http://www.engadget.com/2006/08/18/moo-be-gone-apple-releases-macbook-smc-firmware-update/">SMC firmware update</a>, while helping my Macbook to run cooler, did not help or make it worst.

<strong>Here are come steps you can take to eliminate all troubleshooting:
</strong>
<ol>
	<li>If you have upgraded your RAM and/or Hard Drive, change them back to the stock components.</li>
	<li>Back up your data and do a fresh install of Mac OS X from your install DVD.</li>
	<li>Do a PMU reset. This involves removing the battery, disconnecting the AC adaptor then holding the Power button down for 5secs. replace the battey and connect the power supply back then restart the machine</li>
	<li>Try resting the PRAM. Option-Command-P-R during startup until you here the chime 3 times.</li>
	<li>With the battery and/or AC adaptor connected, hold down the Power Button for until you here a loud chime. This seems to help me when I cant get the system to boot.</li>
	<li>After all this, startup a Terminal window and run the command "yes &gt; /dev/null" then start another Terminal and run the same command. Let this run for about 15mins. Your Macbooks fans should kick in during this time.  This will strain the CPUs and a lot of times you will get a shutdown during or shortly after this.</li>
	<li>If your still having random reboots after all this, contact <a href="http://www.apple.com/support/contact/">Applecare</a> for a repair.</li>
</ol>
I've done all this and have yet to contact Applecare. My Macbook is my only computer and I reply on it for work and personal. I've been trying to find a older G4 machine, iBook or Mac Mini to hold me over while this would be away getting repaired but apparently Mac's hold their value very well. I can' seen to find anything reasonable to hold me over. So right now I'm kinda stuck and not sure what my next step is. According to the forums over at Apple, replacing the logic board doesn't work and the problem will resurface. I had mine for 3 months before it started so who knows if people who aren't having issues after a board replacement will see problems down the road.

I am not alone in this issue either.

<strong>Here are some links to others having the same problem:</strong>
<ul>
	<li><a href="http://theappleblog.com/2006/08/29/random-acts-of-shut-down/">The Apple Blog</a></li>
	<li><a href="http://techpaedia.com/apple/2006/08/21/macbook-random-shut-down/">The Apple Files</a></li>
	<li><a href="http://www.macbookrandomshutdown.com/">www.macbookrandomshutdown.com</a></li>
	<li><a href="http://discussions.apple.com/category.jspa?categoryID=218&amp;start=15#threads">Apple.com Fourms</a></li>
	<li><a href="http://www.powerpage.org/archives/2006/08/macbook_shutdowns.html">O'Grady</a></li>
</ul>
These are just a few. If anyone else is having this problem, drop me a comment and let me know how you made out or if anyone has a good deal on a Mac I could use as a replacement while this is back at Applecare, let me know.

<!-- technorati tags start -->
<!-- technorati tags end -->
