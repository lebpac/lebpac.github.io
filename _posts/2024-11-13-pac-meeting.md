---
layout: post
title: PAC Meeting
tag: 2024-2025
---
{% capture minutes_file %}meetings/{{ page.date | date: "%Y-%m-%d" }}-pac-minutes.pdf{% endcapture %}

{% include pdf.html file=minutes_file name="Meeting Minutes" %}