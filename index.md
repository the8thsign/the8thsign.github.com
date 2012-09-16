---
layout: default
title: Alec Peden
---

{% for post in site.posts limit:5 %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<h4>{{ post.date | date: "%A, %B %d, %Y" }}</h4>
{{ post.content }}
{% endfor %}