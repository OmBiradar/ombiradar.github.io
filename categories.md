---
layout: page
title: Categories
permalink: /categories/
---

<style>
  .category-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 1.5rem;
    margin-top: 2rem;
  }
  .category-card {
    border: 1px solid var(--border-color, #e8e8e8);
    border-radius: 8px;
    padding: 1.5rem;
    text-align: center;
    transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
    background-color: var(--background-color, #fff);
    text-decoration: none !important; /* Force remove underlines */
    color: inherit;
    display: block;
  }
  .category-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 6px 16px rgba(0,0,0,0.08);
  }
  .category-card h2 {
    margin: 0 0 0.5rem 0;
    font-size: 1.5rem;
  }
  .category-card p {
    margin: 0;
    color: var(--text-color, #828282);
    font-size: 0.95rem;
  }
  
  /* Basic dark mode compatibility */
  @media (prefers-color-scheme: dark) {
    .category-card {
      border-color: #444;
      background-color: #222;
    }
    .category-card:hover {
      box-shadow: 0 6px 16px rgba(255,255,255,0.05);
    }
    .category-card p {
      color: #aaa;
    }
  }
</style>

<div class="category-grid">
  {% for category in site.categories %}
    <a href="{{ site.baseurl }}/category/{{ category[0] }}/" class="category-card">
      <h2>{{ category[0] | capitalize }}</h2>
      <p>{{ category[1].size }} post{% if category[1].size != 1 %}s{% endif %}</p>
    </a>
  {% endfor %}
</div>
