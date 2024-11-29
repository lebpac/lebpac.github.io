---
layout: page
title: Meetings
---
{% capture ordinal -%}
{% case post.date | date: "%-d" %}
  {% when '1' or '21' or '31' %}st
  {% when '2' or '22' %}nd
  {% when '3' or '23' %}rd
  {% else %}th
{% endcase %}
{% endcapture %}

You can find upcoming PAC meetings on the [calendar]({% link calendar.md %}). Meetings are held in person in the school library and online via Zoom.

## Minutes

{% include link.html link="https://drive.google.com/drive/folders/1cXYcP6r-JS9iND2MxebtMhN7xCuAapDp" text="📁 Meeting Minutes" %}

### Archive

{% assign postsByTag = site.posts | group_by_exp: "post", "post.tag" %}
{% for tag in postsByTag %}
<h4>{{ tag.name }} school year</h4>
<ul>
  {% for post in tag.items %}
  <li><a href="{{ post.url }}">{{ post.title }}, {{ post.date | date: "%B %-d" }}{{ordinal}}</a></li>
  {% endfor %}
</ul>
{% endfor %}