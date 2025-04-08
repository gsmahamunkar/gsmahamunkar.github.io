---
layout: default
title: "Blog"
permalink: /blog/
---

<div class="blog-container">
  <h1>{{ page.title }}</h1>
  <div class="post-cards">
    {% for post in site.posts %}
    <div class="post-card">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
      <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <a class="read-more" href="{{ post.url | relative_url }}">Read more →</a>
    </div>
    {% endfor %}
  </div>
</div>
