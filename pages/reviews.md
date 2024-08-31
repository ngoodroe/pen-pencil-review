---
layout: table_wrapper
title: Reviews
permalink: /reviews/
---

# Reviews

Here are all the posts:

<div class="list-group">
  {% for post in site.posts %}
    <a href="{{ post.url | relative_url }}" class="list-group-item list-group-item-action">
      <h5 class="mb-1">{{ post.title }}</h5>
      <p class="mb-1">{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </a>
  {% endfor %}
</div>
