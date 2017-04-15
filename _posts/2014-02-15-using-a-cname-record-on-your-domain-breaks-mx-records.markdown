---
layout: post
title: Using a CNAME Record on your Root Domain Breaks MX records
date: '2014-02-15 19:54:00'
tags:
- tips
---

~~**Update:** I am no longer using Ghost and have switched to Jekyll, but this is still useful for anyone that might run into the same problem.~~

**Update #2:** I switched back to Ghost.  They now offer a desktop app which I believe is awesome.

I am using the [Ghost hosted platform](https://ghost.org/pricing/).  They support custom domains and I wanted to use my root domain (eduardobautista.com) instead of a subdomain (www.eduardobautista.com).  Ghost advises against doing this but I was not sure why; they are not that clear about the reason.

So despite their warning, I went ahead and did it anyway.  That's how I found out that when you add a CNAME record on the root domain, it will no longer use your dns records.  I found out about this when I was expecting an email and it never arrived (I use MX records on my domain because I use Google apps).

So that is why my blog is located at www.eduardobautista.com instead of just eduardobautista.com.
