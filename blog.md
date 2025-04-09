---
layout: page
title: Blog
permalink: /blog/
---

<div class="featured-post">
  {% assign featured = site.posts.first %}
  <h2><a href="{{ featured.url | relative_url }}">{{ featured.title }}</a></h2>
  <p class="post-meta"><strong>{{ featured.date | date: "%B %d, %Y" }}</strong></p>
  <p>{{ featured.excerpt | strip_html | truncatewords: 50 }}</p>
  <a class="read-more" href="{{ featured.url | relative_url }}">Read full post →</a>
</div>

<hr style="margin: 40px auto; width: 80%;">

<div class="blog-list">
  {% for post in site.posts offset:1 %}
  <article class="blog-post-card">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta"><strong>{{ post.date | date: "%B %d, %Y" }}</strong></p>
    <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    <a class="read-more" href="{{ post.url | relative_url }}">Read more →</a>
  </article>
  <hr>
  {% endfor %}
</div>
