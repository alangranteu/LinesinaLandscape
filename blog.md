---
title: Slow Trains, Fast Walk, and vice versa - Blog
description: A blog about exploring by train and on foot, especially in Málaga province
layout: default
---

# Blog Archive

{% for post in site.posts %}
 
 <div class="blogentry">
 
   <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
   <p class="postdate">
   {% if post.date %}
     {{ post.date | date_to_string }} 
     {% if post.last_modified_at %}
       &nbsp;(updated {{ post.last_modified_at | date_to_string }}) 
     {% endif %}
   {% endif %}
   </p>
   <p>{{ post.description}}</p>
   <img src= "{{ post.image.path}}" alt="{{ post.image.alt}}"/>

 </div>

{% endfor %}


