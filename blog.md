---
layout: default
title: Blog
permalink: /blog/
---

<div class="blog-banner">
  <img src="/assets/images/blog-banner.jpg" alt="ブログバナー">
</div>

<div class="blog-container">
  <h1>最新記事一覧</h1>
  <ul>
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <span>{{ post.date | date: "%Y-%m-%d" }}</span>
      </li>
    {% endfor %}
  </ul>
</div>
