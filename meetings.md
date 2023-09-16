---
layout: page
title: Meetings
rank: 70
---

You can find upcoming PAC meetings on the [calendar]({% link calendar.md %}). Subscribe to the [mailing list]({% link mailing-list.md %}) and we'll send you instructions on how to join prior to each meeting.

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