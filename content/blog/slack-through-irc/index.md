---
title: Using Slack Through an IRC Client
date: '2019-01-12'
---

It’s no secret that Slack has mixed reviews. On one hand, people talk about how it has improved the experience of chatting inside of an organization, while others say that it is slow (Electron) and is moving us away from more open alternatives such as IRC.

As a freelancer, I don’t believe I would be able to switch all of my clients to use alternatives such as [Twist](https://twist.com) which has native applications. Instead, I tried to find different ways to access my Slack messages.

I recalled that Slack had an IRC gateway, but I later found out that it was removed. I thought that ruled out using IRC to communicate with Slack, but I then found out that [IRCCloud](https://www.irccloud.com) has a [feature that connects to Slack](https://blog.irccloud.com/slack-integration/) and makes the messages available through IRC. _This even works when you use IRCCloud as a bouncer_. This allowed me to access my Slack messages with _a native client_. Yes, _native_, not a glorified web app installed on your computer.

Unfortunately, you do have to pay $5 a month to access this feature and it’s still in beta. You also do not have access to your previous messages, only those going forward. I also had some issues reconnecting using the IRC client I was using (Textual 7), so I switched the IRCCloud web app for now. However, it is _much_ faster than the standard Slack app, even when using the IRCCloud web app.

We are probably stuck with Slack for a while longer. This workflow is not ideal and your data is still trapped within Slack. Hopefully open standards will improve enough so that people who are not tech savvy are able to use them in the future.
