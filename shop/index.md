---
layout: page
title: Магазин
permalink: /shop/
---

# Магазин

Здесь вы можете приобрести мои книги, курсы и другие материалы, которые помогут в развитии вашего ребенка.

<div class="products-grid">
  {% for product in site.products %}
    <div class="product-card">
      {% if product.image %}
      <img src="{{ product.image }}" alt="{{ product.title }}" class="product-image">
      {% endif %}
      <h2><a href="{{ product.url | relative_url }}">{{ product.title }}</a></h2>
      <p>{{ product.excerpt | strip_html | truncatewords: 30 }}</p>
      {% if product.price %}
        <p class="price">{{ product.price }}</p>
      {% endif %}
      <a href="{{ product.url | relative_url }}" class="button">Подробнее</a>
      {% if product.button_url %}
        <a href="{{ product.button_url }}" class="button primary">{{ product.button_text | default: "Купить" }}</a>
      {% endif %}
    </div>
  {% endfor %}
</div> 