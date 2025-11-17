---
layout: default
title: "KaelbleSec Blog – Deutsch"
lang: de
permalink: /de/
---

<h1>Posts</h1>

<ul>
  {% assign posts_de = site.posts | where:"lang","de" %}
  {% for post in posts_de %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span> – {{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>
