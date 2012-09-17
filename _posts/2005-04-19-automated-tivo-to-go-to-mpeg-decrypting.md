---
layout: post
title: 'Automated TiVo To Go to MPEG Decrypting'
tags:
  - convert
  - dvr
  - mce
  - mpeg2
  - tivo
  - tivotogo

---

###Automated TiVo To Go to MPEG Decrypting###


**UPDATED: 8/20/05:**
Looks like Moonlight XMuxer Pro was updated and breaks my graphedit filter. Should be an easy fix but instead of fixing it, i'm going to redirect you to use <a href="http://prish.com/etivo/tbr.htm" onclick="javascript:urchinTracker ('/outbound/article/prish.com');">Direct Show Dump</a> from the guys at eTivo. This program is made to go .tivo to mpg conversions without all the hacks like with autodrvconvert. No filters to install either. I've switched to this myself. Only problem so far is the 'Watched Folders' option isn't working for me. Once that is fixed, it will be perfect for my usage. I'd suggest everyone to take a look at it and give it a try. If people still want me to update the filters and whatnot with autodrvconvert then i will.

**UPDATED: 6/20/05:**
Updated to work with Tivo Desktop 2.1 which eliminates the need for a password.

Preparatory steps...

You will need the DirectShow GraphEdit and the following DirectShow Filters:

* Tivo DirectShow Filter Source (Tivo Desktop 2.1)
* MPEG2 Demuxer (Included)
* MPEG2 Multiplexer (Moonlight M71 recommended)
* Dump (Included)

Step by Step:

1. Download "<a href="http://www.the8thsign.com/download/auto_ttg.zip">AutoDVRConvert with TivoToGo filter</a>
2. Install "<a href="http://www.elecard.com/ftp/pub/Xmuxer/xmuxer_pro_pr.zip">Moonlight XMuxer Pro</a>"
3. Open "DirectShow Filters" and double click "Register Filters.bat"
4. Copy the contents of "AutoDVRconvert" folder to your Tivo Recordings folder
5. Double click to open "AutoDVRconvert.exe"
6. Set the following settings:

Filter Graph to Use: TTG.xgr
Input Path: "your Tivo recoding folder"
Output Path: "your Tivo recoding folder" or any other folder you >want
Input File Extension: tivo
Output File Extension: mpg
Check "AutoStart Auto Converter"

7. Click Apply Settings
8. Restart AutoDVRConvert.exe

Now open up Tivo Desktop and pick some programs to transfer. You can also disable "Auto Converter" and just manually convert files using the "Convert Single File" button on the top.  I did not write the Autodvrconvert.exe program, Heimiko from <a href="http://www.thegreenbutton.com/community/shwmessage.aspx?ForumID=26&amp;MessageID=98810">www.thegreenbutton.com</a> originally created it for use with MCE DVR-MS files. I merely put two and two together, made a new XGR file and documented it.

Few Known issues:
1. Auto convert errors out when you select multiple Tivo shows from Tivo Desktop. Work around is to delete the 0 byte MPEG files after everything is converted and it will restart.
2. Program locks the .TIVO files until you close it. You wont be able to delete the .tivo files until you close Autodrvconvert.exe
3. "Delete original after conversion "setting doesn't work

<a href="http://www.the8thsign.com/download/auto_ttg.zip" class="btn btn-large btn-primary">Download</a>
