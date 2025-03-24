---
layout: service
title: Онлайн-консультации
---

<style>
.consultation-container {
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

.help-list {
  background-color: #f8f8f8;
  padding: 20px 30px;
  border-radius: 10px;
  border-left: 4px solid #00a09c;
  margin: 30px 0;
}

.help-list li {
  margin-bottom: 10px;
  list-style-type: none;
  position: relative;
  padding-left: 25px;
}

.help-list li:before {
  content: "✓";
  position: absolute;
  left: 0;
  color: #00a09c;
  font-weight: bold;
}

.consultation-cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin: 30px 0;
  gap: 20px;
}

.consultation-card {
  flex: 1 0 100%;
  background: white;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
  margin-bottom: 20px;
  padding: 30px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  border: 1px solid #eee;
}

.consultation-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 30px rgba(0, 0, 0, 0.12);
}

.card-title {
  color: #333;
  margin-top: 0;
  font-size: 24px;
  border-bottom: 1px solid #eee;
  padding-bottom: 15px;
}

.price-tag {
  font-size: 28px;
  font-weight: bold;
  color: #ff5252;
  margin: 15px 0;
}

.highlight {
  background: linear-gradient(to right, rgba(255, 225, 0, 0.1), rgba(255, 225, 0, 0.7) 4%, rgba(255, 225, 0, 0.3));
  font-weight: bold;
  padding: 0.1em 0.4em;
  margin: 0 -0.4em;
  border-radius: 0.8em 0.3em;
  box-decoration-break: clone;
  -webkit-box-decoration-break: clone;
}

.consultation-button {
  display: inline-block;
  margin-top: 20px;
  padding: 12px 30px;
  background-color: #00a09c;
  color: white;
  font-weight: bold;
  text-align: center;
  text-decoration: none;
  border-radius: 30px;
  transition: all 0.3s ease;
  border: none;
  font-size: 16px;
  cursor: pointer;
  width: 100%;
}

.consultation-button:hover {
  background-color: #008b87;
  transform: translateY(-3px);
  box-shadow: 0 4px 10px rgba(0, 160, 156, 0.3);
}

@media (max-width: 768px) {
  .consultation-cards {
    flex-direction: column;
  }
  
  .consultation-card {
    flex: 1 0 100%;
  }
}
</style>

<div class="consultation-container">

<h1 class="page-title">Консультации</h1>

<h2 class="section-title">Я могу помочь, если...</h2>

<ul class="help-list">
  <li>вы заметили <span class="highlight">отклонения</span> в развитии своего ребёнка и не знаете, куда обратиться.</li>
  <li>вы видите <span class="highlight">аутистические признаки</span> у своего ребенка, но не знаете, что делать</li>
  <li>у вашего ребенка диагноз <span class="highlight">аутизм</span> и вы не знаете, как заниматься с ним дома</li>
  <li>ваш ребенок <span class="highlight">непоседливый и неусидчивый</span> и у вас не получается с ним заниматься</li>
  <li>у вас ребенок 1.5 - 5 лет и он отстает в <span class="highlight">речи и коммуникации</span> от нормы</li>
  <li>у ребенка <span class="highlight">нет указательного жеста</span>, а ему уже есть 15 месяцев</li>
  <li>вам кажется, что ребенок <span class="highlight">не понимает</span> обращенную речь</li>
</ul>

<h2 class="section-title">Варианты консультаций</h2>

<div class="consultation-cards">
  <div class="consultation-card">
    <h3 class="card-title">Консультация</h3>
    <p class="price-tag">40 €</p>
    <p>Сессия включает предварительный анализ видеозаписи поведения и коммуникации ребенка, час консультации по видео через Telegram или WhatsApp.</p>
    <p>Я отвечу на все ваши вопросы, расскажу конкретно, что <span class="highlight">делать дальше</span>, дам детальные задания и объясню методики <span class="highlight">для коррекции вашего ребенка</span> дома.</p>
    <p>Оплатить можно любой картой MasterCard и Visa, а так же через PayPal.</p>
    <a href="https://www.instagram.com/toy_kina/" class="consultation-button">Записаться на консультацию<br/>(директ в Инстаграм)</a>
  </div>
  
  <div class="consultation-card">
    <h3 class="card-title">Консультация + <u>программа</u></h3>
    <p class="price-tag">50 €</p>
    <p>Сессия включает предварительный анализ видеозаписи поведения и коммуникации ребенка, час консультации по видео через Telegram или WhatsApp, а так же составление индивидуальной программы (pdf) с занятиями для развития вашего ребенка на 4 месяца.</p>
    <p>Я отвечу на все ваши вопросы, расскажу конкретно, что <span class="highlight">делать дальше</span>, а после консультации пришлю большую <span class="highlight">индивидуальную программу</span> с занятиями для вашего ребенка, по которой вы сможете самостоятельно проводить <span class="highlight">домашнюю коррекцию</span>.</p>
    <p>Оплатить можно любой картой MasterCard и Visa, а так же через PayPal.</p>
    <a href="https://www.instagram.com/toy_kina/" class="consultation-button">Записаться на консультацию<br/>(директ в Инстаграм)</a>
  </div>
</div>

<h2 class="section-title">Как проходит консультация</h2>

<ol>
  <li>Вы связываетесь со мной через директ в Instagram (@toy_kina)</li>
  <li>Мы договариваемся о дате и времени консультации</li>
  <li>Вы заранее отправляете мне видеозаписи поведения и коммуникации вашего ребенка</li>
  <li>В назначенное время я связываюсь с вами через Telegram или WhatsApp</li>
  <li>Консультация длится 1 час, во время которой я отвечаю на все ваши вопросы</li>
  <li>Если вы выбрали пакет с программой, я отправляю вам индивидуальную программу в течение 3-5 дней после консультации</li>
</ol>

</div> 