---
layout: post
title: 'How to setup up AUTD on Exchange 2003 with T-Mobile MPx220'
tags:
  - activesync
  - autd
  - exchange
  - motorola
  - mpx220
  - smartphone
  - tmobile

---

Finally got away from the PDA / Cellphone combo I always carried around with the purchase of my new Motorola MPx220 Smartphone. The MPx220 runs Microsoft's Windows Mobile 2003SE software which virtually replaces my iPaq 2215 and Nokia 3650. This is how to setup a new MPx220 to work with Push based Activesync over T-Mobile's GPRS network. What this means is every time a new email, appointment or contact is added to your Exchange the server will "push" it to you phone in a matters of minutes without you having to sync manually. This is done by the Exchange server sending out a SMS message that the phone receives (and deletes immediately) and this initializes a server Activesync connect. With this in mind, i highly suggest you get the $19.99 Unlimited Internet plan with a 1000 SMS bucket for $6.99 from T-Mobile.

-----------------

**Exchange 2003 setup:**

1. Install Exchange 2003 Service Pack 1 if you haven't already
2. Follow the registry edit in <a href="http://support.microsoft.com/?kbid=841995">this KB article </a>
3. Install <a href="http://www.the8thsign.com/download/Exchange2003-KB841995-x86-enu.exe">this hotfix</a>
4. Start Exchange System Manager
5. Open Organization > Global Services
6. Click Mobile Services
7. Goto Action > New > Mobile Carrier
8. Type in T-Mobile as the carrier name
9. Type "@tmomail.net" for the SMTP Domain
10. Close out all windows



**MPx220 Connection Settings**

1. Start > Settings > More > Data Connections
2. Press Menu > Edit Connections
3. Go down to GPRS Connections
4. Menu > Add  
Fill in as following:  
Description: T-Mobile GPRS  
Connects to: The Internet  
Access Point: wap.voicestream.com  
Leave the rest blank  
5. Hit Done Twice
6. Goto Proxy Connections
7. Menu > Add
Fill in as following:  
Description: T-Mobile GPRS  
Connects from: The Internet  
Connects to: WAP Network  
Proxy: 216.155.165.50:8080  
Type: HTTP  
Leave rest blank  
8. Click Done until your back at your Homescreen
9. Start > Internet Explorer > Menu > Options > Connections
10. Select Network : WAP Network

**Setup Activesync on MPx220**

1. Start > Activesync
2. Menu > Options > Server Settings > Connections
Fill in as following:  
User Name: [your exchange username]  
Password: [your exchange password]  
Domain: [your windows domain]  
Check Save Password  
Server Name: [your server ie mail.yourdomain.com]  
Check Use SSL Connection  
3. Click Done until your back at the Active Screen
4. Menu > Server Settings
5. Click Inbox > Check Sync Inbox with a Server then set your options as you see fit
6. Click Calender > Check "Sync Calender with a Server" then set your options as you see fit
7. Click Contact > Check "Sync Contacts with a Server"
8. Click Done to your back to Activesync screen
9. Sync - Hopefully it should connect and sync for the first time.
10. Menu > Options > Mobile Schedule
11. Change the "Peak time sync" to "When new items arrive"
12. Change the "Off-peak time sync" to "When new items arrive"
13. Sync again
14. Menu > Options > Server Settings > Connections
15. Scroll down to Address device using  
Fill in as follows:  
Address device using: SMTP Address  
Service Provider Name: T-Mobile (should be auto-filled)  
Device Phone Number: [your mobile number]  
Text Message Address: [yourmobilenumber]@tmomail.net  
18. Click Done til your at Activesync screen
17. Sync