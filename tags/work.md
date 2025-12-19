---
layout: default
title: Work
permalink: /tags/work/
---

# Work

{% if site.tags.work %}
  {% for post in site.tags.work %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%d %b %Y" }}
  {% endfor %}
{% else %}
_No posts yet._
{% endif %}
