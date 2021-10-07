---
layout: post
title: PAC Meeting
tag: 2020-2021
---
{% capture minutes_file %}meetings/{{ page.date | date: "%Y-%m-%d" }}-pac-minutes.pdf{% endcapture %}

{% include pdf.html file=minutes_file name="Meeting Minutes" %}

{% include pdf.html file="meetings/2020-09-03-chat-log.pdf" name="Chat Log" %}