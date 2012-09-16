---
layout: default
title: Alec Peden
---

{% for post in site.posts limit:5 %}
<a href="{{ post.url }}">{{ post.title }}</a>
{{ post.date | date: "%A, %B %d, %Y" }}
{{ post.content }}
{% endfor %}