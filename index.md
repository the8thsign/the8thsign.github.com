---
layout: default
title: Alec Peden
---

{% for post in site.posts limit:5 %}
<h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
<i class="icon-time"></i>{{ post.date | date: "%A, %B %d, %Y" }}
{{ post.content }}
{% endfor %}
<hr>


