---
layout: default
title: Alec Peden
---

{% for post in site.posts limit:5 %}
<div class="posttitle"><a href="{{ post.url }}">{{ post.title }}</a></div>
<div class="date">{{ post.date | date: "%A, %B %d, %Y" }}</div>
{{ post.content }}
{% endfor %}