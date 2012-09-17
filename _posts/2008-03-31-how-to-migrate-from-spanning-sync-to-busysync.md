---
layout: post
title: 'How to migrate from Spanning Sync to BusySync'
tags:
  - busysync
  - calendar
  - google
  - spanningsyc

---

<p><img src="http://www.the8thsign.com/wp-content/uploads/2008/03/main-image2.jpg" alt="main-image2.jpg" border="0" width="500" height="258" /></p>

<p>My one year subscription to <a href="http://spanningsync.com/">Spanning Sync</a> is coming up and while I've been very happy with the program itself, the $25 a year or $65 one time fee doesn't. Last year I opted for the one year subcription as Leopard hadn't been released and I was hoping for some built in support for syncing iCal to Google. Well that didn't happen. This year at Macworld, <a href="http://www.busymac.com/">BusyMac</a> showed off a beta of BusySync 2.0 which supports syncing to Google Calendar... all for $19.95 for 1.x and a free upgrade 2.0 when released. Thanks to a 50% coupon code, Google Calendar syncing only costs me $9.98. Due to the different way each program uses to sync iCal and Google Calendar, its not as straight forward to switch to BusySync. </p>

<p>1) Backup. This is the most important step. Go to iCal > File > Export and save each of you calendars.</p><img src="http://www.the8thsign.com/wp-content/uploads/2008/03/picture-1.png" alt="Picture 1.png" border="0" width="335" height="296" />
<p>2) Disable .Mac calendar Syncing - You should not use both BusySync and .Mac to sync calendars between the same Macs. This will end up causing you to have duplicate calendars.</p> 
<img src="http://www.the8thsign.com/wp-content/uploads/2008/03/picture-4.png" alt="Picture 4.png" border="0" width="393" height="291" />
<p>3) Turn off Spanning Sync. Make one last sync with Spanning Sync then go into System Preferences > Spanning Sync and uncheck the "Sync with Google Calendar" box.</p><img src="http://www.the8thsign.com/wp-content/uploads/2008/03/picture-5.png" alt="Picture 5.png" border="0" width="500" height="445" />
<p>4) Decided where you want to "host" your calendars. This is where most of the work is done. Spanning Sync requires you to create parallel calendars in iCal and Google Calendar and map them to each other. BusySync uses a Publish and Subscribe model where one side is the host and the other side is the client. We will need to delete any calendars that are not the host. In my example, I had 2 calendars in iCal, one called Home and Work. Google Calendar had 2 calendars called Alec Peden (default calendar that you cannot delete) and Work. I mapped Home > Alec Peden and Work > Work. To BusySync, that would be 4 different calendars. We only need 2. Since you cannot delete the default calendar in Google Calendar, we will want to delete the calendar in iCal that you had mapped to it. In my case, it would be the Home calendar. All the other calendars you have, you just need to decide where you want the host calendar to be and delete the corresponding calendar. Since I use Time Machine to back up iCal, I decided on using iCal's calendars as the host. It honestly does not matter which one you decide.</p>
<p>3) Install BusySync 2.0.</p> <img src="http://www.the8thsign.com/wp-content/uploads/2008/03/picture-6.png" alt="Picture 6.png" border="0" width="500" height="427" />
<p>4) Setup which calendars to sync by going to the System Preferences > BusySync and click the Google tab. Place a check mark next to the calendars you want to sync. Keep in mind you can have host calendars in both iCal and Google Calendar. To read more about which calendar is the client and host, <a href="http://www.busymac.com/faqs.html%23google-host">visit BusySync</a>.</p>
<img src="http://www.the8thsign.com/wp-content/uploads/2008/03/picture-2.png" alt="Picture 2.png" border="0" width="500" height="411" />
<p>5) Sync. Everything should be setup and ready to sync. Your first sync may take a few minutes but you should start to see the calendars you checked show up in both iCal and Google Calendar. If everything worked out the way you want it, go ahead and uninstall Spanning Sync by Ctrl+Clicking the icon in System Preferences and choose "Remove".</p>

<p><strong>Note</strong>: If you run into any problems. Delete the problem calendar(s), recreate a new blank calendar in either iCal or Google Calendar, check the box to sync it in BusySync and once its sync, import the ICS backup you made in step 1 into iCal.</p>



