---
layout: page
title: Meetings
---

## Upcoming

Join the [mailing list]({% link mailing-list.md %}) to get notified about upcoming meetings.

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