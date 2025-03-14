---
layout: page
title: Магазин
permalink: /shop/
---

<style>
.shop-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.section-heading {
  text-align: center;
  position: relative;
  margin-bottom: 40px;
  color: #333;
}

.section-heading:after {
  content: "";
  position: absolute;
  bottom: -15px;
  left: 50%;
  width: 100px;
  height: 3px;
  background-color: #00a09c;
  transform: translateX(-50%);
}

.section-description {
  text-align: center;
  max-width: 800px;
  margin: 0 auto 50px;
  color: #555;
  font-size: 18px;
  line-height: 1.6;
}

.products-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
  gap: 30px;
  margin-top: 40px;
}

.product-card {
  background: white;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
  transition: all 0.3s ease;
  display: flex;
  flex-direction: column;
  height: 100%;
}

.product-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 15px 30px rgba(0, 0, 0, 0.12);
}

.product-image-container {
  height: 240px;
  overflow: hidden;
}

.product-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.5s ease;
}

.product-card:hover .product-image {
  transform: scale(1.05);
}

.product-content {
  padding: 25px;
  display: flex;
  flex-direction: column;
  flex-grow: 1;
}

.product-title {
  margin-top: 0;
  margin-bottom: 15px;
  font-size: 24px;
}

.product-title a {
  color: #333;
  text-decoration: none;
  transition: color 0.3s ease;
}

.product-title a:hover {
  color: #00a09c;
}

.product-excerpt {
  color: #666;
  line-height: 1.6;
  margin-bottom: 20px;
  flex-grow: 1;
}

.price {
  font-size: 28px;
  font-weight: bold;
  color: #ff5252;
  margin: 15px 0;
}

.product-buttons {
  margin-top: auto;
  display: flex;
  gap: 10px;
}

.button {
  padding: 12px 20px;
  text-decoration: none;
  border-radius: 30px;
  font-weight: bold;
  text-align: center;
  transition: all 0.3s ease;
  flex: 1;
}

.button:hover {
  transform: translateY(-3px);
}

.primary {
  background-color: #00a09c;
  color: white;
}

.primary:hover {
  background-color: #008b87;
  box-shadow: 0 4px 10px rgba(0, 160, 156, 0.3);
}

.button:not(.primary) {
  background-color: #f5f5f5;
  color: #333;
  border: 1px solid #ddd;
}

.button:not(.primary):hover {
  background-color: #eee;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

@media (max-width: 768px) {
  .products-grid {
    grid-template-columns: 1fr;
  }
  
  .product-buttons {
    flex-direction: column;
  }
}
</style>

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