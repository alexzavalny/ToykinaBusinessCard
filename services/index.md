---
layout: page
title: Услуги
permalink: /services/
logo: /img/logo-teach.jpg
---

<div class="services-container">
  <h2 class="section-heading">Мои услуги</h2>
  <p class="section-description">Я предлагаю различные форматы работы, чтобы вы могли выбрать наиболее подходящий для вас и вашего ребенка.</p>

  <div class="services-grid">
    {% for service in site.services %}
      <div class="service-card">
        <div class="service-content">
          <h3 class="service-title"><a href="{{ service.url | relative_url }}">{{ service.title }}</a></h3>
          <p class="service-excerpt">{{ service.excerpt | strip_html | truncatewords: 30 }}</p>
          {% if service.price %}
            <p class="service-price">{{ service.price }}</p>
          {% endif %}
        </div>
        <div class="service-actions">
          <a href="{{ service.url | relative_url }}" class="button">Подробнее</a>
        </div>
      </div>
    {% endfor %}
  </div>
</div> 