---
layout: page
title: Meetings
---

{% comment %}
## Upcoming events

<iframe src="https://calendar.google.com/calendar/embed?height=480&wkst=1&bgcolor=%23ffffff&ctz=America%2FVancouver&showTitle=0&showTz=0&showCalendars=0&showTabs=0&showPrint=0&showDate=1&showNav=1&mode=MONTH&src=bGFwZWJwYWNAZ21haWwuY29t&color=%237986CB" style="border-width:0" width="720" height="480" frameborder="0" scrolling="no"></iframe>
{% endcomment %}

## Meeting minutes

{% assign postsByTag = site.posts | group_by_exp: "post", "post.tag" %}
{% for tag in postsByTag %}
<h3>{{ tag.name }} school year</h3>
<ul>
  {% for post in tag.items %}
  <li><a href="{{ post.url }}">{{ post.title }}, {{ post.date | date: "%Y-%m-%d" }}</a></li>
  {% endfor %}
</ul>
{% endfor %}