---
layout: page
title: Услуги
permalink: /services/
---

# Мои услуги

Я предлагаю различные форматы работы, чтобы вы могли выбрать наиболее подходящий для вас и вашего ребенка.

<div class="services-grid">
  {% for service in site.services %}
    <div class="service-card">
      <h2><a href="{{ service.url | relative_url }}">{{ service.title }}</a></h2>
      <p>{{ service.excerpt | strip_html | truncatewords: 30 }}</p>
      {% if service.price %}
        <p class="service-price">{{ service.price }}</p>
      {% endif %}
      <a href="{{ service.url | relative_url }}" class="button">Подробнее</a>
    </div>
  {% endfor %}
</div> 