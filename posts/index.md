---
layout: default
title: Posts
---

<h1>Posts</h1>

{% assign albums = site.posts | group_by: "album" %}

{% for album in albums %}
  <h2>{{ album.name }}</h2>
  <div class="visual-grid">
    {% for post in album.items %}
      <a href="{{ post.url | relative_url }}">
        <img src="{{ post.image }}" alt="{{ post.title }}" loading="lazy" />
      </a>
    {% endfor %}
  </div>
{% endfor %}

<p><a href="{{ '/' | relative_url }}" class="back-home pulse-hover">&larr; Back to home</a></p>
