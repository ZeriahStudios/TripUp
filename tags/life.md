---
layout: default
title: Life
permalink: /tags/life/
---

# Life

{% if site.tags.life %}
  {% for post in site.tags.life %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%d %b %Y" }}
  {% endfor %}
{% else %}
_No posts yet._
{% endif %}
