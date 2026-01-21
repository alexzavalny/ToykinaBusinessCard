---
layout: page
title: Магазин
permalink: /shop/
logo: /img/logo-shop.jpg
---

<style>
.shop-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.shop-layout {
  display: flex;
  gap: 40px;
  align-items: flex-start;
}

.shop-sidebar {
  flex: 0 0 260px;
}

.shop-sidebar .sidebar-section {
  background-color: #f8f8f8;
  border-radius: 12px;
  padding: 20px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
  position: sticky;
  top: 30px;
}

.shop-sidebar .sidebar-heading {
  margin: 0 0 15px;
  font-size: 20px;
  color: #333;
  border-bottom: 1px solid #e0e0e0;
  padding-bottom: 10px;
}

.shop-category-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.shop-category-list li {
  margin-bottom: 10px;
}

.shop-category-link {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 14px;
  border-radius: 8px;
  color: #333;
  text-decoration: none;
  transition: background-color 0.2s ease, color 0.2s ease;
}

.shop-category-link .category-count {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 12px;
  padding: 2px 8px;
  font-size: 0.85rem;
}

.shop-category-link:hover {
  background-color: #e9f5f4;
  color: #008b87;
}

.shop-category-link.active {
  background-color: #d1f2ef;
  color: #00726f;
  font-weight: 600;
}

.shop-content {
  flex: 1;
}

.mobile-category-toggle {
  display: none;
  justify-content: center;
  gap: 12px;
  margin-bottom: 20px;
}

.category-toggle-button {
  background-color: #00a09c;
  color: #fff;
  border: none;
  border-radius: 30px;
  padding: 10px 24px;
  font-weight: bold;
  cursor: pointer;
  display: flex;
  align-items: center;
  gap: 8px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  transition: background-color 0.2s ease;
}

.category-toggle-button .toggle-icon {
  transition: transform 0.2s ease;
}

.category-toggle-button.open .toggle-icon {
  transform: rotate(180deg);
}

.category-toggle-button:hover {
  background-color: #008b87;
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

@media (max-width: 992px) {
  .shop-layout {
    flex-direction: column;
  }
  
  .shop-sidebar {
    width: 100%;
    display: none;
  }
  
  .shop-sidebar.active {
    display: block;
  }
  
  .shop-sidebar .sidebar-section {
    position: static;
  }
  
  .mobile-category-toggle {
    display: flex;
  }
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
  <div class="mobile-category-toggle">
    <button id="shop-category-toggle" class="category-toggle-button">
      Категории <span class="toggle-icon">▼</span>
    </button>
  </div>

  <div class="shop-layout">
    <aside class="shop-sidebar" id="shop-sidebar">
      <div class="sidebar-section">
        <h3 class="sidebar-heading">Категории</h3>
        <ul class="shop-category-list">
          <li>
            <a href="{{ '/shop/' | relative_url }}" class="shop-category-link category-all active" data-category="all" data-label="Магазин">
              Все товары
              <span class="category-count">{{ site.products | size }}</span>
            </a>
          </li>
          {% assign shop_categories = "Пособия,Игры,Курсы,Книги" | split: "," %}
          {% for category in shop_categories %}
            {% assign trimmed_category = category | strip %}
            {% assign encoded_category = trimmed_category | url_encode %}
            {% assign category_products = site.products | where: "category", trimmed_category %}
            <li>
              <a href="{{ '/shop/' | relative_url }}#category-{{ encoded_category }}" class="shop-category-link" data-category="{{ encoded_category }}" data-label="{{ trimmed_category }}">
                {{ trimmed_category }}
                <span class="category-count">{{ category_products | size }}</span>
              </a>
            </li>
          {% endfor %}
        </ul>
      </div>
    </aside>

    <div class="shop-content">
      <h2 class="section-heading">Магазин</h2>
      <p class="section-description">Здесь вы можете приобрести мои книги, курсы и другие материалы, которые помогут в развитии вашего ребенка.</p>

      <div class="products-grid">
        {% for product in site.products %}
          <div class="product-card" data-category="{{ product.category | default: 'Прочее' | url_encode }}">
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
  </div>
</div>

<script>
  document.addEventListener('DOMContentLoaded', function() {
    var basePath = '{{ "/shop/" | relative_url }}';
    var categoryLinks = document.querySelectorAll('.shop-category-link');
    var productCards = document.querySelectorAll('.product-card');
    var sidebar = document.getElementById('shop-sidebar');
    var toggleButton = document.getElementById('shop-category-toggle');
    var sectionHeading = document.querySelector('.shop-content .section-heading');
    var defaultHeading = sectionHeading ? sectionHeading.textContent.trim() : '';

    function setActiveLink(category) {
      categoryLinks.forEach(function(link) {
        link.classList.remove('active');
      });

      if (category === 'all') {
        var allLink = document.querySelector('.shop-category-link.category-all');
        if (allLink) {
          allLink.classList.add('active');
        }
      } else {
        var targetLink = document.querySelector('.shop-category-link[data-category="' + category + '"]');
        if (targetLink) {
          targetLink.classList.add('active');
        }
      }
    }

    function updateHeading(category) {
      if (!sectionHeading) {
        return;
      }
      if (category === 'all') {
        sectionHeading.textContent = defaultHeading || 'Магазин';
        return;
      }
      var targetLink = document.querySelector('.shop-category-link[data-category="' + category + '"]');
      if (targetLink) {
        var label = targetLink.getAttribute('data-label') || targetLink.textContent.trim();
        sectionHeading.textContent = label;
      }
    }

    function filterCategory(category) {
      productCards.forEach(function(card) {
        var cardCategory = card.getAttribute('data-category');
        if (category === 'all' || cardCategory === category) {
          card.style.display = '';
        } else {
          card.style.display = 'none';
        }
      });
      setActiveLink(category);
      updateHeading(category);
    }

    function showAllProducts() {
      filterCategory('all');
    }

    function applyFilterFromHash() {
      var hash = window.location.hash;
      if (hash && hash.indexOf('#category-') === 0) {
        var category = hash.replace('#category-', '');
        filterCategory(category);
      } else {
        showAllProducts();
      }
    }

    categoryLinks.forEach(function(link) {
      link.addEventListener('click', function(event) {
        var targetCategory = this.dataset.category;
        if (!targetCategory) {
          return;
        }
        event.preventDefault();

        if (targetCategory === 'all') {
          history.replaceState(null, '', basePath);
          showAllProducts();
        } else {
          window.location.hash = 'category-' + targetCategory;
        }

        if (sidebar) {
          sidebar.classList.remove('active');
        }
        if (toggleButton) {
          toggleButton.classList.remove('open');
        }
      });
    });

    if (toggleButton && sidebar) {
      toggleButton.addEventListener('click', function() {
        sidebar.classList.toggle('active');
        this.classList.toggle('open');
      });
    }

    window.addEventListener('hashchange', applyFilterFromHash);
    applyFilterFromHash();
  });
</script>
