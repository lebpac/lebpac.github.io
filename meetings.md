---
layout: page
title: Meetings
---

## Upcoming

Join the [mailing list]({% link mailing-list.md %}) to get notified about upcoming meetings.

* October 20, 2021
* November 18, 2021
* January 20, 2022
* February 24, 2022
* April 21, 2022
* May 18, 2022
* June 16, 2022

Oct 20th (Weds); Nov 18th (Thurs); Jan 20 (Thurs); Feb 24th (Thurs); April 21 (Thurs); May 18th (Weds); June 16th (Thurs)

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