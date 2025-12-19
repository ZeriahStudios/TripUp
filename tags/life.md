---
layout: default
title: Life
permalink: /tags/life/
---

# Life

{% assign items = site.posts | where_exp: "p", "p.tags contains 'life'" %}

{% if items.size == 0 %}
_No posts yet._
{% else %}
<ul>
  {% for post in items %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> — {{ post.date | date: "%d %b %Y" }}</li>
  {% endfor %}
</ul>
{% endif %}
