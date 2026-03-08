---
layout: post
title: Blog
permalink: /blog/
is_blog: true
---

<div class="blog-list">
  <ul>
    {% for post in site.posts %}
      {% unless post.categories contains "read" %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a> – {{ post.date | date: "%B %d, %Y" }}
        </li>
      {% endunless %}
    {% endfor %}
  </ul>
</div>