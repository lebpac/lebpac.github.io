---
layout: post
title: AGM Meeting
tag: 2018-2019
---
{% capture minutes_file %}meetings/{{ page.date | date: "%Y-%m-%d" }}-agm-minutes.pdf{% endcapture %}

{% include pdf.html file=minutes_file name="Meeting Minutes" %}

{% include pdf.html file="meetings/2019-06-17-budget.pdf" name="2019-2020 Budget" %}