---
layout: post
title: PAC Meeting
tag: 2021-2022
---
{% capture minutes_file %}meetings/{{ page.date | date: "%Y-%m-%d" }}-pac-minutes.pdf{% endcapture %}

{% include pdf.html file=minutes_file name="Meeting Minutes" %}

{% include pdf.html file="meetings/2021-09-23-budget.pdf" name="2021-2022 Proposed Budget" %}