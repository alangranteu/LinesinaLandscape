---
title: Slow Trains, Fast Walk, and vice versa - Blog
description: A blog about exploring by train and on foot, especially in Málaga province
---

# Blog Archive

{% for post in site.posts %}
 
 <div class="blogentry">
 
   <h4><a href="{{ post.url }}">{{ post.title }}</a>/h4>
   <p>
   Published {{ page.date | date_to_long_string }} 
   {% if page.updated %}
     Last updated {{ page.updated | date_to_long_string }} 
   {% endif %}
   </p>
   <p>{{ post.description}}</p>
   <a href="{{ post.url }}"> <img src= "{{ post.image.path}}" alt="{{ post.image.alt}}"/></a>

 </div>

{% endfor %}


