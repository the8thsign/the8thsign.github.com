---
layout: default
title: Alec Peden
---

{% for post in site.posts limit:5 %}
<div class="span8">
    <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
    {{ post.content }}
    <div>
        <span class="badge badge-success">{{ post.date | date: "%A, %B %d, %Y" }}</span><div class="pull-right"><span class="label">alice</span> <span class="label">story</span> <span class="label">blog</span> <span class="label">personal</span></div>
    </div> 
    {% endfor %}