---
title: Blog - Slow Trains Fast Walks (and vice versa) - Blog
description: A blog about exploring by train and on foot, especially in Málaga province
---

# Blog Archive

{% for post in site.posts %}
  <p><a href="{{ post.url }}">{{ post.title }}</a><br>
  {{ post.date | date_to_string }}<br>
  {{ post.description}}<br>
  [test image]({{ post.image}})</p>
{% endfor %}