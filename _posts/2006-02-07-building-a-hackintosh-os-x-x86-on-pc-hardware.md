---
layout: post
title: 'Building a Hackintosh - OS X x86 on PC hardware'
tags:
  - apple
  - diy
  - hackintosh
  - hardware
  - howto
  - osx
  - osx86
  - pc
  - shopping
  - switch

---

Here is what i used to get OS X 10.4.3 x86 up and running using PC components as my everyday PC. This should last me until the Intel Mac Minis are released and I can actually get my hands on a real Mac.

I used macosx_10.4.3_8f1111_for_dtk_userdvd.dmg, converted it to ISO using <a href="http://www.ezbsystems.com/ultraiso/">UltraISO</a> and then patched it with <a href="http://rapidshare.de/files/10120119/1111a.Generic.Patch.v4.2b.zip.html">JaS 1111a Generic Patch v4.2b PPF</a>. Burned it to DVD and that part was done. Next was putting together the hardware.

Motherboard: <a href="http://www.newegg.com/Product/Product.asp?Item=N82E16813186083">Foxconn 915GL7MH-S Socket T (LGA 775) Intel 915GL Micro ATX Intel Motherboard - Retail</a> - $66
CPU: <a href="http://www.newegg.com/Product/Product.asp?Item=N82E16819112205">Intel Celeron D 336 Prescott 533MHz FSB LGA 775 64-Bit Processor w/ Execute Disable Bit Model BX80547RE2800CN - Retail</a> - $89
Memory: <a href="https://www.zipzoomfly.com/jsp/ProductDetail.jsp?ProductCode=80098-6">Corsair VS512MB400 512MB DDR400 PC3200 CAS2.5 Value Select Memory Retail</a> x2 - $40.99
Hard Drive: <a href="https://www.zipzoomfly.com/jsp/ProductDetail.jsp?ProductCode=100719-4">Maxtor DiamondMax 10 6L300S0 300GB Serial ATA 7200RPM Hard Drive w/16MB Buffer</a> - $123.99
DVDROM: <a href="https://www.zipzoomfly.com/jsp/ProductDetail.jsp?ProductCode=171025">Pioneer DVR-110 16X Dual Layer DVD�RW Drive (Black)</a> - $46.50
Case: Generic from local PC shop - $65
Keyboard: Apple Pro Keyboard - $29

Total: $501.47

Alright, now that we got our PC ready, its time to install. Now I've read a bunch of different methods to install involving partitioning with partition magic, windows diskpart, using vmware etc. I didn't need any of that.

1) Boot up the PC with the DVD in the drive and set to boot.
2) At the Installation Screen, goto Tools &gt; Disk Utility.
3) Choose the drive on the right.
4) Click the Partition button and choose 1 Partition from the drop-down menu. Hit the Partition button on the bottom to partition the drive.
5) Close Disk Utility and continue the install.
5) Click on the Customize button and Uncheck the Developer Tools and whatever printer drivers you don't need.
6) Finish Installing.

Problems i ran into:
While USB keyboard and Mouse worked during the install, it didn't after first boot. I had to use a PS2 Keyboard and Mouse to finish the setup then deleted AppleFPMemDriver.kext and AppleTPMACPI.kext from the Extensions directory. After that i rebooted with USB keyboard and mouse plugged in an they worked with no problem after that.

Sound output only works out of Line-Out, not Speaker-Out.
<!-- technorati tags start -->
<!-- technorati tags end -->
