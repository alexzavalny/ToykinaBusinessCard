---
layout: page
title: Магазин
permalink: /shop/
---

<div class="shop-container">
  <h2 class="section-heading">Магазин</h2>
  <p class="section-description">Здесь вы можете приобрести мои книги, курсы и другие материалы, которые помогут в развитии вашего ребенка.</p>

  <div class="products-grid">
    {% for product in site.products %}
      <div class="product-card">
        {% if product.image %}
        <div class="product-image-container">
          <img src="{{ product.image }}" alt="{{ product.title }}" class="product-image">
        </div>
        {% endif %}
        <div class="product-content">
          <h3 class="product-title"><a href="{{ product.url | relative_url }}">{{ product.title }}</a></h3>
          <p class="product-excerpt">{{ product.excerpt | strip_html | truncatewords: 30 }}</p>
          {% if product.price %}
            <p class="price">{{ product.price }}</p>
          {% endif %}
          <div class="product-buttons">
            <a href="{{ product.url | relative_url }}" class="button">Подробнее</a>
            {% if product.button_url %}
              <a href="{{ product.button_url }}" class="button primary">{{ product.button_text | default: "Купить" }}</a>
            {% endif %}
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
</div> 