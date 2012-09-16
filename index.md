---
layout: default
title: Alec Peden
---

{% for post in site.posts limit:5 %}
    <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
    {{ post.content }}
    {% endfor %}