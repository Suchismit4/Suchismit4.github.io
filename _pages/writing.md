---
layout: page
title: writing
permalink: /writing/
nav: true
nav_order: 2
---

Notes on machine learning, research systems, and computational methods will appear here.

{% if site.posts.size > 0 %}
{% for post in site.posts %}

- {{ post.date | date: '%Y-%m-%d' }} · [{{ post.title }}]({{ post.url | relative_url }})
  {% endfor %}
  {% endif %}
