---
layout: default
title: Home
---

<div class="hero">
  <div class="big">Trip Up</div>
  <p>Capture repeatable human mistakes so others don’t have to make them again.</p>
  <div class="quote"><em>Mistakes repeat across people, not destinations.</em></div>
</div>

<hr>

## Featured Trip Ups

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%d %b %Y" }}
{% endfor %}
