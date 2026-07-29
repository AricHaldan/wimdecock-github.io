---
layout: page
title: Artikels
description: Een verzameling van mijn schrijfsels
---

<ul class="articles-list">
{% raw %}{% assign sorted = site.articles | sort: 'date' | reverse %}
{% for item in sorted %}
  <li>
    <h2><a href="{{ item.url }}">{{ item.title }}</a></h2>
    <p class="date">{{ item.date | date: "%B %-d, %Y" }}</p>
    <p>{{ item.excerpt | strip_html | truncatewords: 40 }}</p>
  </li>
{% endfor %}{% endraw %}
</ul>
[back](./)
