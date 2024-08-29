---
layout: default
title: main page 
---

Hello, we are amazing people, a group of eccentric lawyers.

{% for post in site.posts %}
  <h2 class="post-title"><a href="{{ post.url | relative_url}}">{{ post.title }} {{ post.date | date: "%e %B %Y" }} </a></h2>
  {% if post.subtitle %}
    <h3 class="post-subtitle">{{post.subtitle}}</h3>
  {% endif %}
  {{ post.content | markdownify | strip_html | truncatewords: 50 }}
  <a href="{{ post.url | relative_url}}">... read more</a>
{% endfor %}
