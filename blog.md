---
title: Blog - Slow Trains Fast Walks (and vice versa) - Blog
description: A blog about exploring by train and on foot, especially in Málaga province
---

# Blog Archive

{% for post in site.posts %}
 
 <a href="{{ post.url }}">{{ post.title }}</a>
 {{ post.date | date_to_string }}
 {{ post.description}}
 ![test image]({{ post.image}})

{% endfor %}

![test alt text](empty.jpg)
