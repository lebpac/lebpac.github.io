---
layout: page
title: Meetings
---

## Upcoming

This year's scheduled PAC meetings:

* November 18, 2021
* January 20, 2022
* February 24, 2022
* April 21, 2022
* May 18, 2022
* June 16, 2022

Meetings take place at **7 pm** on **Zoom**. Subscribe to the [mailing list]({% link mailing-list.md %}) and we'll send you instructions on how to join prior to each meeting.

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