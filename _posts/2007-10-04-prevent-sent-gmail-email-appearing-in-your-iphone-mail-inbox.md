---
layout: post
title: 'Prevent Gmail Sent Email From Appearing in Your iPhone Mail Inbox'
tags:
  - gmail
  - google
  - iphone

---

Using iPhone and your Gmail account? Then you have certainly noticed the annoying phenomenon of your send messages showing up in your iPhone Inbox. Luckily, I have seen this problem before with my Blackberry and was able to fix it. Unlucky for you, there is no fix for this on the iPhone. I repeat, THERE IS NO FIX.

Apple has a support document which outlines this problem and how to fix it <a href="http://docs.info.apple.com/article.html?artnum=305937" target="_blank">here</a>. This only fixes part of a bigger problem. First we need to understand what Recent mode is. This is right from Google's Help page:
<blockquote> If you're accessing your Gmail using POP from multiple clients, Gmail's recent mode makes sure that all messages are made available to each client, rather than only to the first client to access new mail.

Recent mode fetches the last 30 days of mail, regardless of whether it's been sent to another POP client already.</blockquote>
If you use multiple Email clients, then Recent Mode is a must and you will want to keep it on. For argument sake, lets say you only access Gmail POP from your iPhone. Turning off Recent Mode will fix one problem, and only one. Sent Email from your iPhone ONLY will not show up. Emails sent from other POP clients and the Web interface still show up in your iPhone's Inbox.

This happens due to the way threaded conversations work in Gmail. With a Blackberry, you can set up a BIS Filter for all emails with your address in the from field to not forward to the Blackberry. We have no such luxury with the iPhone since it doesn't support filters. And don't listen to the people who say to create a filter in Gmail to delete your send messages. It will prevent the emails from showing up but the messages will get emptied from the Trash after 30 days and threaded conversations will no longer be useful.

As of now we have a few half-assed workarounds that degrade Gmail functionality. So unless Apple updates the iPhone with an internal filter when using Gmail or Google releases full IMAP support, us Gmail/iPhone users are stuck with this.
