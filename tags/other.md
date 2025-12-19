---
layout: default
title: Other
permalink: /tags/other/
---

# Other

{% if site.tags.other %}
  {% for post in site.tags.other %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%d %b %Y" }}
  {% endfor %}
{% else %}
_No posts yet._
{% endif %}
