---
layout: post
title: Reads
permalink: /read/
---



<div class="read-grid">
  {% for post in site.posts %}
    {% if post.categories contains "read" %}
      <div class="read-card">
        <a href="{{ post.url }}">
          <img src="{{ post.cover }}" alt="{{ post.title }}">
        </a>
        <p>{{ post.title }}</p>
        <div class="rating">
          {% case post.rating %}
            {% when 5 %}★★★★★
            {% when 4 %}★★★★☆
            {% when 3 %}★★★☆☆
            {% when 2 %}★★☆☆☆
            {% when 1 %}★☆☆☆☆
            {% else %}☆☆☆☆☆
          {% endcase %}
        </div>
      </div>
    {% endif %}
  {% endfor %}
</div>

<style>


.read-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr); /* 3 cards per row */
  gap: 1rem;
  margin-top: 2rem;
}

.read-card {
  text-align: center;
  transition: 0.3s ease;
}

.read-card img {
  width: 50%;   /* fill the grid cell */
  border-radius: 10px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s;
}

.read-card img:hover {
  transform: scale(1.05);
}

.read-card p {
  margin-top: 0.5rem;
  font-weight: bold;
  font-size: 0.95rem;
}

.rating {
  margin-top: 0.25rem;
  font-size: 1.8rem;
  color: #FFD700; /* Gold stars */
  letter-spacing: 1px;
}
</style>







