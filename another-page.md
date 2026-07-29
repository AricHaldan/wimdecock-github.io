---
layout: default
title: Artikels
description: Een verzameling van mijn schrijfsels
---

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%B %-d, %Y" }}</p>
  <p>{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
{% endfor %}

[back](/)
