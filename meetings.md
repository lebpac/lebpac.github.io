---
layout: page
title: Meetings
---

You can find upcoming PAC meetings on the [calendar]({% link calendar.md %}). Meetings are generally held from 7–8 pm in the school library.

## Minutes

{% assign postsByTag = site.posts | group_by_exp: "post", "post.tag" %}
{% for tag in postsByTag %}
<h3>{{ tag.name }} school year</h3>
<ul>
  {% for post in tag.items %}
  <li><a href="{{ post.url }}">{{ post.title }}, {{ post.date | date: "%Y-%m-%d" }}</a></li>
  {% endfor %}
</ul>
{% endfor %}