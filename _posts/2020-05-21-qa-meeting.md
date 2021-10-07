---
layout: post
title: Q&A Session
tag: 2019-2020
---
{% capture minutes_file %}meetings/{{ page.date | date: "%Y-%m-%d" }}-qa.pdf{% endcapture %}

{% include pdf.html file=minutes_file name="Meeting Minutes" %}