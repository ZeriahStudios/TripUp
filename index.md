---
layout: default
title: Home
permalink: /
---

<div class="hero">
  <div class="big">Trip Up</div>
  <p>Capture repeatable human mistakes so others don’t have to make them again.</p>
  <div class="quote"><em>Mistakes repeat across people, not destinations.</em></div>
</div>

## Browse by Category

<div class="cardgrid">
  {% for c in site.data.categories %}
    <a class="card" href="{{ c.href | relative_url }}">
      <div class="pill">{{ c.badge }}</div>
      <div class="card-title">{{ c.title }}</div>
      <div class="card-desc">{{ c.desc }}</div>
    </a>
  {% endfor %}
</div>

<hr>

## Featured Trip Ups

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%d %b %Y" }}
{% endfor %}
