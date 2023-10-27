---
title: Blog - Slow Trains Fast Walks (and vice versa) - Blog
description: A blog about exploring by train and on foot, especially in Málaga province
---

{% for post in site.posts %}
  <p><a href="{{ post.url }}">{{ post.title }}</a><br>
  {{ post.excerpt }}<br>
  {{ post.date | date_to_string }}</p>
{% endfor %}