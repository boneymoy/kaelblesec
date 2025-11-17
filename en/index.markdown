---
layout: default
title: "KaelbleSec Blog – English"
lang: en
permalink: /en/
---

<h1>Posts</h1>

<ul>
  {% assign posts_en = site.posts | where:"lang","en" %}
  {% for post in posts_en %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span> – {{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>
