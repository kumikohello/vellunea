---
layout: default
title: Posts
---

<h1>Posts</h1>

<nav>
  <a href="{{ '/about/' | relative_url }}" class="pulse-hover">about</a>
  <a href="{{ '/music/' | relative_url }}" class="pulse-hover">music</a>
  <a href="{{ '/posts/' | relative_url }}" class="active" class="pulse-hover">posts</a>
  <a href="{{ '/visuals/' | relative_url }}" class="pulse-hover">visuals</a>
  <a href="{{ '/contact/' | relative_url }}" class="pulse-hover">contact</a>
</nav>

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

<p><a href="{{ '/' | relative_url }}" class="back-home">&larr; Back to home</a></p>
