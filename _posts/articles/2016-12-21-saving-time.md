---
layout: post
title: Saving Time
excerpt: "Do you waste too much time on Reddit, Youtube etc?"
categories: personal
tags: [productivity]
comments: true
share: true
---

The internet provides you with an endless supply of content to kill time on

My choice of poisons are Reddit and Youtube but this cannot go on, so it's time to make it a bit inconvinient to get on those sites

Opening links from your history seems to bypass the hosts file(bug?) so clear out your history too

```shell
    nuke@mistborn ~ $ cat /etc/hosts
    127.0.0.1 localhost
    127.0.1.1 mistborn
    127.0.1.1 reddit.com
    127.0.1.1 youtube.com
```