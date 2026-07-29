---
layout: default
title: Artikels
description: Een verzameling van mijn schrijfsels
---

## Opiniestukken

[A Brave New Censorship](https://docs.google.com/document/d/1pYUpLMWhKAAfjCoaMDaAFruFjnvyplH1tWcwuCh7Mu8/edit?usp=sharing).

On the 25th of July, the UK has rolled out new measures to enforce their digital safety act which have vastly changed how British citizens have experienced the internet. This law has had increasingly absurd consequences such as being unable to access Spotify without giving away your personal information and uploading your ID and face to prove that you’re an adult. It may even lead to Wikipedia being inaccessible to UK readers...

<ul class="posts-list">
{% raw %}{% assign sorted = site.posts | sort: 'date' | reverse %}
{% for item in sorted %}
  <li>
    <h2><a href="{{ item.url }}">{{ item.title }}</a></h2>
    <p class="date">{{ item.date | date: "%B %-d, %Y" }}</p>
    <p>{{ item.excerpt | strip_html | truncatewords: 40 }}</p>
  </li>
{% endfor %}{% endraw %}

[back](./)
