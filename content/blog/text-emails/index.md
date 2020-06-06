---
title: Please Write Multipart Emails for your Newsletters
date: '2019-02-06'
---

Ever since deciding to permanently disable images on all the emails I receive (even from people I trust), I occasionally run into the inconvenience of viewing an email with a bunch of blank squares where I suppose a huge image is supposed to be.  Just an image, and almost no text to explain what the email is about.  This is a shame because I do sometimes subscribe to newsletters on purpose because I want to stay up to do date with a service that I am using.

Now, I am definitely *not* going to enable images just for these emails.  I disabled images as a matter of principal against all of the tracking that happens when an email is opened.  But *you* can write a [multipart email](https://www.w3.org/Protocols/rfc1341/7_2_Multipart.html).

Basically, you can send a rich HTML email, with a plain text alternative for those of us who prefer plain text.  Rails already supports multipart emails and I imagine many other web frameworks as well.  Services such as Mailchimp also support multipart emails so there really isn't an excuse not to include a plain text version in your next newsletter.
