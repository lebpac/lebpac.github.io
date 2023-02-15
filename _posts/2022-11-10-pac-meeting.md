---
layout: post
title: PAC Meeting
tag: 2022-2023
---
{% capture minutes_file %}meetings/{{ page.date | date: "%Y-%m-%d" }}-pac-minutes.pdf{% endcapture %}

{% include pdf.html file=minutes_file name="Meeting Minutes" %}