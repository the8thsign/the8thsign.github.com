---
layout: post
title: 'Linksys WRTSL54GS and Mac OS X'
tags:
  - apple
  - howto
  - linksys
  - macosx
  - osx
  - wrtsl54gs

---

Anyone using a USB hard drive connected to Linksys's WRTSL54GS Router and Mac OS X may come across an error that reads <em>The operation cannot be completed because you do not have sufficient privileges for some of the items</em> when trying to copy files to the USB hard drive. If copying one file, it will finish copying but you will receive the error at the end. When copying multiply files, the first file will copy then you will receive the error and no more files will copy.

<img src="http://www.the8thsign.com/wp-content/uploads/2006/04/error-2-tm.jpg" alt="Error-2" border="1" height="100" hspace="4" vspace="4" width="369" />

This only happens in OS X and more specifically, Finder. If you copy files using terminal, they will copy fine. I'm not exactly sure of the cause of it but it has to so with the SMB server and permissions. Problem is, since the SMB server is running through firmware on the router, we can't do in and make changes. I've used hacked firmwares with telnet access and still cant get chown to work. So that leaves us with using a workaround on OS X's side. There really is two ways of doing this. Both are similar.

First the hard way:

Since all the files on the USB HDD connected to the WRTSL54GS are owned by root, we will make a root account on the router.
<ol>
	<li>Login to your router using its IP address, usually 192.168.1.1</li>
	<li>Click on the Storage Tab, then click on Administration</li>
	<li>First we are going to create a new group, name it root</li>
	<li>Next make a new user called root and add them to the root group</li>
	<li>Connect to your shares on the WRTSL54GS using �oot as your username</li>
</ol>
<img src="http://www.the8thsign.com/wp-content/uploads/2006/04/admin-1-tm.jpg" alt="Admin-1" border="1" height="393" hspace="4" vspace="4" width="488" />

or a second way, and easier way, to do this is to use the built in admin account by setting a password for the admin account. Do this under Storage &gt; Administration and not the Administration tab as that will change the router password. After that is set, when you connect to any share on the WRTSL54GS, make sure you login using admin as your username and use the password you set. No more error message.

<!-- technorati tags start -->
<!-- technorati tags end -->
