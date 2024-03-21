---
title: Blog
description: A blog about exploring by train and on foot, especially in Málaga province
layout: default
---

# Blog Archive

{% for post in site.posts %}
 
 <div class="blogentry">
 
   <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
   <p class="postdate">
   {% if post.date %}
     {{ post.date | date_to_string }} 
     {% if post.last_modified_at %}
       &nbsp;(updated {{ post.last_modified_at | date_to_string }}) 
     {% endif %}
   {% endif %}
   </p>
   <p>{{ post.description}}</p>
   {% if post.image.path %}
      <a href="{{ post.url }}"><img src= "{{ post.image.path}}" alt="{{ post.image.alt}}"></a>
   {% endif %}
 </div>

{% endfor %}


