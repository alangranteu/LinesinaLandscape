---
title: Blog - Slow Trains Fast Walks (and vice versa) - Blog
description: A blog about exploring by train and on foot, especially in Málaga province
---

# Blog Archive

{% for post in site.posts %}
 
 <div class="blogentry">
 <a href="{{ post.url }}">{{ post.title }}</a>
 <br>{{ post.date | date_to_string }}
 <br>{{ post.description}}
 <br><a href="{{ post.url }}" <img src= "{{ post.image}}" alt="{{ post.image.alt}}"/></a>

</div>

{% endfor %}


