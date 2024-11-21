---
layout: default
title: Chess Grandmaster Blog
---

# Welcome to the Chess Grandmaster Blog

Explore the fascinating world of chess through strategic insights, game analyses, and personal reflections. Join me on a journey through the 64 squares of strategy, skill, and intellectual challenge.

## Latest Blog Posts

{% for post in site.posts limit:3 %}
  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
    <small>Posted on {{ post.date | date: "%B %d, %Y" }}</small>
  </article>
{% endfor %}