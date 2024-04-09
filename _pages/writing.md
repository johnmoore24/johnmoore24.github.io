---
layout: default
title: Writing
permalink: /writing/
---

<div class="posts-list">
  {% for post in site.posts %}
    <article class="post">
      <h2>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      </h2>
      <p class="post-meta">{{ post.date | date: '%b %-d, %Y' }}</p>
      <p class="excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
    </article>
  {% endfor %}
</div>
