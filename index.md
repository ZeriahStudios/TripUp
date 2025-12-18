---
layout: default
title: Home
---

## What is Trip Up?

Trip Up captures **repeatable human mistakes** so others don’t have to make them again.

> *Mistakes repeat across people, not destinations.*

---

## Featured Trip Ups

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
