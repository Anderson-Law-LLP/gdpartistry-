---
layout: default
title: main page 
---

Hello, we are working on an interesting project which involves building a blog site to discuss GDPR! 

WELCOME TO GDPARGH!

{% for post in site.posts %}
  <h2><a href="{{ post.url | relative_url}}">{{ post.title }}</a></h2>
  {% if post.subtitle %}
    <h3>{{post.subtitle}}</h3>
  {% endif %}
{% endfor %}
