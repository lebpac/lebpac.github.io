---
layout: page
title: Meetings
---

You can find upcoming PAC meetings on the [calendar]({% link calendar.md %}). Afternoon meetings are held in person in the school library and online. Evening meetings are online only.

Everyone is welcome.

{% include link.html link="https://drive.google.com/drive/folders/1cXYcP6r-JS9iND2MxebtMhN7xCuAapDp" text="📁 Meeting Agendas & Minutes" %}

{% include link.html link="https://meet.google.com/knu-aurw-hxm" text="![Google Meet](/assets/img/meet_icon.svg) Join online via Google Meet" %}

## Archive

{% assign postsByTag = site.posts | group_by_exp: "post", "post.tag" %}
{% for tag in postsByTag %}
<h4>{{ tag.name }} school year</h4>
<ul>
  {% for post in tag.items %}
  <li><a href="{{ post.url }}">{{ post.title }}, {{ post.date | date: "%B %-d" }}</a></li>
  {% endfor %}
</ul>
{% endfor %}