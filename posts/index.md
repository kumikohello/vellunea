---
layout: default
title: Posts
---

<h1>Posts</h1>

<div class="instagram-grid">
  {% for url in site.data.featured_instagram %}
    {% include instagram_embed.html url=url %}
  {% endfor %}
</div>

<p><a href="{{ '/' | relative_url }}" class="back-home pulse-hover">&larr; Back to home</a></p>
