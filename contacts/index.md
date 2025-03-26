---
layout: page
title: Контакты
permalink: /contacts/
logo: /img/logo-contact.jpg
---

<style>
.contact-container {
  max-width: 800px;
  margin: 0 auto;
  padding: 0 20px;
}

.section-title {
  border-bottom: 2px solid #00a09c;
  padding-bottom: 10px;
  color: #333;
  margin-top: 40px;
}

.contact-cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin-top: 30px;
}

.contact-card {
  width: 100%;
  max-width: 350px;
  margin-bottom: 25px;
  padding: 20px;
  background: linear-gradient(160deg, #f8f8f8, #fff);
  border-radius: 10px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.contact-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
}

.contact-icon {
  font-size: 36px;
  color: #00a09c;
  margin-bottom: 15px;
}

.contact-link {
  display: inline-block;
  color: #00a09c;
  font-weight: bold;
  text-decoration: none;
  margin-top: 10px;
  padding: 5px 0;
  border-bottom: 2px solid transparent;
  transition: border-color 0.3s ease;
}

.contact-link:hover {
  border-color: #00a09c;
}

.social-list {
  background-color: #f8f8f8;
  padding: 20px 30px;
  border-radius: 10px;
  border-left: 4px solid #00a09c;
  margin: 30px 0;
}

.social-list li {
  margin-bottom: 15px;
  list-style-type: none;
  position: relative;
  padding-left: 30px;
}

.social-list li:before {
  content: "➤";
  position: absolute;
  left: 0;
  color: #00a09c;
}

.page-title {
  text-align: center;
  position: relative;
  margin-bottom: 40px;
}

.page-title:after {
  content: "";
  position: absolute;
  bottom: -15px;
  left: 50%;
  width: 100px;
  height: 3px;
  background-color: #00a09c;
  transform: translateX(-50%);
}

.contact-description {
  text-align: center;
  max-width: 600px;
  margin: 0 auto 40px auto;
  color: #555;
  font-size: 18px;
  line-height: 1.6;
}

@media (max-width: 768px) {
  .contact-cards {
    justify-content: center;
  }
  
  .contact-card {
    max-width: 100%;
  }
}
</style>

<div class="contact-container">

<h1 class="page-title">Свяжитесь со мной</h1>

<p class="contact-description">Вы можете связаться со мной любым удобным для вас способом. Я всегда рада помочь и ответить на ваши вопросы о развитии вашего ребенка.</p>

<div class="contact-cards">
  <div class="contact-card">
    <div class="contact-icon">✉️</div>
    <h3>Телеграм</h3>
    <p>Самый быстрый способ связаться со мной - написать в Телеграм.</p>
    <a class="contact-link" href="https://t.me/toyechkina" target="_blank">@toyechkina</a>
  </div>
  
  <div class="contact-card">
    <div class="contact-icon">📷</div>
    <h3>Инстаграм</h3>
    <p>Следите за обновлениями и полезной информацией в моем Инстаграме.</p>
    <a class="contact-link" href="https://instagram.com/toy_kina" target="_blank">@toy_kina</a>
  </div>
</div>

<h2 class="section-title">Мои ресурсы</h2>

<ul class="social-list">
  <li>
    <strong>Телеграм-канал</strong>: 
    <a href="https://t.me/toy_kina" target="_blank">t.me/toy_kina</a> - 
    здесь я публикую полезные материалы и развивающие упражнения
  </li>
  <li>
    <strong>YouTube</strong>: 
    <a href="https://www.youtube.com/@toy_kina" target="_blank">youtube.com/@toy_kina</a> - 
    канал с интервью с экспертами и демонстрацией методик
  </li>
</ul>

</div>
