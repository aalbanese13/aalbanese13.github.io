---
layout: page
title: Blog
permalink: /blog/
---
<ul class="blog-list">
{% for post in site.posts %}
  <li class="blog-item">
      <h2 class="post-title">{{ post.title }}</h2>

      <h5 class="post-date">{{ post.date | date: "%b %-d, %Y" }}</h5>

      <p class="post-excerpt">{{ post.excerpt }}</p>

      <a class="read-more" href="{{ post.url }}">
      Read More
      </a>
  </li>
{% endfor %}
</ul>
