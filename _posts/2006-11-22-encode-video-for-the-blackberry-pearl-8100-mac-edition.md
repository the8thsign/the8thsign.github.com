---
layout: post
title: 'Encode Video for the Blackberry Pearl 8100: Mac edition'
tags:
  - automator
  - blackberry
  - howto
  - osx
  - software

---

Since I got my 1GB MicroSD card for my Pearl, I've been toying around with trying to get Videos to work. Either the videos don't look good, dont play at all or lag the controls. The best method I've found so far was using mencoder but due to its command line usage and not being able to find a UB for it made it difficult to encode videos. This is where this guide come in.

<strong>Getting Started</strong>

1) First off this is the command line we will be using:
<em>"mencoder -vf scale=240:-10 &lt;input.file&gt; -o &lt;output.file&gt; -of avi -ofps 15 -ovc lavc -oac lavc -lavcopts vcodec=mpeg4:vbitrate=230:acodec=mp3:abitrate=64"
</em>
2) <a href="http://www.the8thsign.com/download/mencoder.zip">Download</a> the Universal Build of mencoder

<strong>Encoding
</strong>
At this point you can just drop the mencoder into the same directory as the file you want to convert, start a terminal window and copy the command line to encode it. Be sure to change the input and output file. In a few mins you should have your video ready to be loaded on your Pearl.  But as Mac users we will want a more elegant way of doing this. Enter Applescript and more importantly Automator.

1) <a href="http://www.the8thsign.com/download/encode_workflow.zip">Download</a> my Automator Workflow (<strong>Updated 3/2/07</strong>)
2) Unzip the file into
"/Users/<em>YOURUSERNAME</em>/Library/Workflows/Applications/Finder/"

3) Unzip mencoder.zip on your Desktop, start up Terminal and type "cd Desktop" then "sudo mv mencoder /usr/bin". Enter your password when prompted too.

3) Now when you Right Click(Ctrl+Click) on a Video file, you will see the Automator Menu and under that you should see "Encode for Blackberry"

4) To encode, just chose "Encode for Blackberry" on a Video file

<strong>Thats it</strong>

The only visual indicator you have is a "Run Shell Script" in the Menu bar.

A Blackperry Pearl compatible file will be created in the same folder as FILENAME-bb.avi. You can edit the Workflow to output to the filename of your choice. You could even go as far as modifying the Automator Workflow to copy the file to your Pearl if you would like.

A 54meg Music Video that runs 3:32mins takes about 30secs to encode on a Macbook 2.0G and the ending file size is about 8megs. Not too bad at all. Most TV shows will be about 50megs for a 30min show and movies are between 150megs to 250megs in my tests. I've also noticed that the mencoder build will not take advantage of Duo Core's.

<span style="text-decoration: line-through"><strong>UPDATE</strong></span><span style="text-decoration: line-through"> - </span><span style="text-decoration: line-through"><strong>12/20/06</strong></span><span style="text-decoration: line-through">
Here is a </span><span style="text-decoration: line-through">widescreen version</span><span style="text-decoration: line-through"> that needs to go through some testing. Please feel free to try it and leave a comment on how it works for you. YMMV</span>

<strong>UPDATE - 02/11/07</strong>
<a href="http://www.askdavetaylor.com/">Dave Taylor</a> has whipped up a <a href="http://www.the8thsign.com/download/convert-avi.sh">shell script</a> that does the same thing if you would like to do the <a href="http://www.askdavetaylor.com/turn_command_line_into_shell_script.html">command line</a> route.

<strong>UPDATE - 3/2/07</strong>
Thanks to Chris for the tip, the Workflow now keeps accept ratio when encoding.

<!-- technorati tags start -->
<!-- technorati tags end -->
