---
layout: default
title: Just Do It! - Archives
---

<!-- <div class="posts-without-bar"> -->
<div class="post">
  <h1 class="pageTitle">Archives</h1>
  <h2 class="pageTitle">GANs</h2>
  <ul class="posts-without-bar">
    {%- for post in site.posts -%}
      {% if post.category == "GAN" %}
        <li>
          <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
          <span class="date">&nbsp;{{ post.date | date: '%B %d, %Y' }}</span>
        </li>
      {% endif %}
    {%- endfor -%}
  </ul>
</div>
