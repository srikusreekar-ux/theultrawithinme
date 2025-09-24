---
layout: default
title: Blog
---

# Blog

Posts are in `_posts/` and appear below automatically.

<ul>
  {% for post in site.posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %d, %Y" }}</li>
  {% endfor %}
</ul>
