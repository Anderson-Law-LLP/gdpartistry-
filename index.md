---
layout: default
title: main page 
---

Hello, we are working on an interesting project which involves building a blog site to discuss GDPR! 

WELCOME TO GDPARGH!

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
