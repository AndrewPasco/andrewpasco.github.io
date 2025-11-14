---
layout: default
title: Blog
permalink: /blog/
---

{% include nav.html %}

# Blog Posts

{% for post in site.blog %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
