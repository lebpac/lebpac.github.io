---
layout: post
title: AGM Meeting
tag: 2020-2021
---
{% capture minutes_file %}meetings/{{ page.date | date: "%Y-%m-%d" }}-agm-minutes.pdf{% endcapture %}

{% include pdf.html file=minutes_file name="Meeting Minutes" %}