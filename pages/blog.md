---
layout: page
title: Blog
permalink: /blog/
---


<ul class="blog-list">
{% for post in site.posts %}
  <li>
      <h3>{{ post.title }}</h3>

      <h5>{{ post.date | date: "%b %-d, %Y" }}</h5>

      <p>{{ post.excerpt }}</p>

      <a href="{{ post.url }}">
      Read More
      </a>
  </li>
{% endfor %}
</ul>
