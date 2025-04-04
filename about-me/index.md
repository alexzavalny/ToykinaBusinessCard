---
layout: page
title: Обо мне
permalink: /about-me/
logo: /img/logo-hi.jpg
---

<style>
.about-container {
  max-width: 800px;
  margin: 0 auto;
  padding: 0 20px;
}

.profile-image-container {
  display: flex;
  justify-content: center;
  margin: 30px 0;
}

.profile-image {
  max-width: 250px;
  border-radius: 50%;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  transition: transform 0.3s ease;
}

.profile-image:hover {
  transform: scale(1.05);
}

.section-title {
  border-bottom: 2px solid #00a09c;
  padding-bottom: 10px;
  color: #333;
  margin-top: 40px;
}

.stats {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin: 30px 0;
  padding: 20px;
  background: linear-gradient(160deg, #f8f8f8, #fff);
  border-radius: 10px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
}

.stats div {
  text-align: center;
  padding: 15px;
  min-width: 150px;
}

.stats-number {
  font-size: 48px;
  font-weight: bold;
  color: #00a09c;
  margin: 0;
}

.stats-label {
  margin-top: 5px;
  font-size: 16px;
  color: #555;
}

.help-list {
  background-color: #f8f8f8;
  padding: 20px 30px;
  border-radius: 10px;
  border-left: 4px solid #00a09c;
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

.approach-list li {
  margin-bottom: 12px;
}

.faq-section {
  background: #f9f9f9;
  padding: 20px 25px;
  border-radius: 10px;
  margin: 30px 0;
}

.faq-section dt {
  font-weight: bold;
  margin-top: 15px;
  color: #333;
}

.faq-section dd {
  margin-left: 0;
  margin-bottom: 15px;
  padding-bottom: 15px;
  border-bottom: 1px solid #eee;
}

.diplomas-section {
  margin: 40px 0;
  padding: 20px;
  background: #f8f8f8;
  border-radius: 10px;
}

.diplomas-shelf {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
  padding: 20px;
  background: #e8e8e8;
  border-radius: 8px;
  box-shadow: inset 0 2px 4px rgba(0,0,0,0.1);
}

.diploma-item {
  background: white;
  padding: 10px;
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
  max-width: 200px;
  cursor: pointer;
  transform: rotate(var(--rotation));
}

.diploma-item:nth-child(1) {
  --rotation: -3deg;
}

.diploma-item:nth-child(2) {
  --rotation: 2deg;
}

.diploma-item:nth-child(3) {
  --rotation: -1deg;
}

.diploma-item:nth-child(4) {
  --rotation: 3deg;
}

.diploma-item:hover {
  transform: rotate(0deg) scale(1.05);
  z-index: 1;
}

.diploma-item img {
  width: 100%;
  height: auto;
  border-radius: 4px;
  object-fit: cover;
}

.diploma-title {
  margin-top: 10px;
  text-align: center;
  font-size: 14px;
  color: #333;
}

.lightbox {
  display: none;
  position: fixed;
  z-index: 999;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.9);
  cursor: pointer;
}

.lightbox-content {
  margin: auto;
  display: block;
  max-width: 90%;
  max-height: 90vh;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.close {
  position: absolute;
  right: 25px;
  top: 10px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
}

.close:hover {
  color: #bbb;
}

.contact-section {
  background-color: #00a09c;
  color: white;
  padding: 20px;
  border-radius: 10px;
  text-align: center;
  margin-top: 40px;
}

.contact-section a {
  color: white;
  font-weight: bold;
  text-decoration: underline;
}

@media (max-width: 600px) {
  .stats {
    flex-direction: column;
  }
  
  .stats div {
    margin-bottom: 20px;
  }
}
</style>

<div class="about-container">


<div class="profile-image-container">
  <img class="profile-image" loading="lazy" src="/img/profile.png?2" alt="Фотография Ксении Тоечкиной" />
</div>

<h2 class="section-title">Обо мне</h2>

Меня зовут Ксения. Мне 35 лет, я из Риги. Я детский нейропсихолог и монтессори-педагог и я занимаюсь развитием детей с различными расстройствами развития (ЗРР, ЗПРР, аутизм, СДВГ, синдром Дауна). Моя основная задача - помогать родителям <strong>самим корректировать</strong> своих детей.

Я помогаю родителям детей с различными расстройствами развития сразу <strong>начать дома коррекцию</strong> развития ребенка не <strong>упуская время</strong>.

<h2 class="section-title">Мой опыт</h2>

<section class="stats">
  <div>
    <p class="stats-number">5</p>
    <p class="stats-label">лет занятий с детьми</p>
  </div>
  <div>
    <p class="stats-number">120+</p>
    <p class="stats-label">учеников</p>
  </div>
  <div>
    <p class="stats-number">170+</p>
    <p class="stats-label">проведенных консультаций</p>
  </div>
</section>

<h2 class="section-title">Я могу помочь, если...</h2>

<ul class="help-list">
  <li>вы заметили <strong>отклонения</strong> в развитии своего ребёнка и не знаете, куда обратиться.</li>
  <li>вы видите <strong>аутистические признаки</strong> у своего ребенка, но не знаете, что делать</li>
  <li>у вашего ребенка диагноз <strong>аутизм</strong> и вы не знаете, как заниматься с ним дома</li>
  <li>ваш ребенок <strong>непоседливый и неусидчивый</strong> и у вас не получается с ним заниматься</li>
  <li>у вас ребенок 1.5 - 5 лет и он отстает в <strong>речи и коммуникации</strong> от нормы</li>
  <li>у ребенка <strong>нет указательного жеста</strong>, а ему уже есть 15 месяцев</li>
  <li>вам кажется, что ребенок <strong>не понимает</strong> обращенную речь</li>
</ul>

<h2 class="section-title">Мой подход</h2>

Я понимаю, что <strong>родителям нелегко разобраться</strong> во всех тонкостях развития ребенка. На своих консультациях я рассказываю родителям как правильно заниматься с ребенком, чтобы <strong>улучшить динамику</strong> его развития.

В своей работе я использую комплексный подход, включающий:

<ul class="approach-list">
  <li>Диагностику особенностей развития ребенка</li>
  <li>Разработку индивидуальной программы коррекции</li>
  <li>Обучение родителей эффективным методикам работы с ребенком</li>
  <li>Регулярное сопровождение и корректировку программы</li>
</ul>

<h2 class="section-title">Ответы на частые вопросы</h2>

<dl class="faq-section">
  <dt>При каких расстройствах я могу помочь?</dt>
  <dd>Я могу помочь при расстройствах, таких как ЗРР (задержка речевого развития), ЗПРР (задержка психического развития), РАС (расстройства аутистического спектра), алалия и СДВГ (синдром дефицита внимания и гиперактивности).</dd>

  <dt>Консультирую ли я про развитие нормотипичных детей?</dt>
  <dd>Да, я консультирую по вопросам развития нормотипичных детей и могу помочь подготовить вашего ребенка к школе.</dd>

  <dt>При каких расстройствах я не могу помочь?</dt>
  <dd>Я не могу помочь при ДЦП (детском церебральном параличе) и при сильной умственной отсталости. Я не помогу, если ребенок картавит или заикается.</dd>

  <dt>Выписываю ли я лекарства?</dt>
  <dd>Нет, я не могу выписывать лекарства, так как я не врач. Я могу дать рекомендации, которые вы сможете обсудить со своим лечащим врачом.</dd>

  <dt>Ставлю ли я диагнозы?</dt>
  <dd>Нет, я не могу ставить диагнозы, так как это прерогатива врача. Я - педагог, и моя основная задача - помочь в составлении программы коррекции развития ребенка.</dd>

  <dt>Зачем нужны видеозаписи поведения ребенка?</dt>
  <dd>Видеозаписи необходимы для того, чтобы я могла лучше понять его поведение, навыки и сложности, с которыми он сталкивается. Это позволяет мне дать более точные и конкретные рекомендации.</dd>

  <dt>Как происходит оплата консультации?</dt>
  <dd>Оплатить можно MasterCard, Visa карточками, а так же через PayPal. Оплата происходит через платежную систему Stripe. Stripe это одна из самых популярных платежных систем в мире, используется на миллионах сайтов. Она позволяет оплачивать услуги и товары, не передавай данные о карточке получателю средств.</dd>
</dl>

<h2 class="section-title">Мои дипломы и сертификаты</h2>

<div class="diplomas-section">
  <div class="diplomas-shelf">
    <div class="diploma-item" onclick="openLightbox(this)">
      <img src="/img/diploma/aba_v1.jpg" alt="Сертификат ABA терапии" loading="lazy">
      <div class="diploma-title">Первый курс ABA Юлии Эрц</div>
    </div>
    <div class="diploma-item" onclick="openLightbox(this)">
      <img src="/img/diploma/aba_v2.jpg" alt="Сертификат ABA терапии" loading="lazy">
      <div class="diploma-title">Второй курс ABA Юлии Эрц</div>
    </div>
    <div class="diploma-item" onclick="openLightbox(this)">
      <img src="/img/diploma/montessori.jpeg" alt="Сертификат Монтессори-педагога" loading="lazy">
      <div class="diploma-title">Сертификат Монтессори-педагога</div>
    </div>
    <div class="diploma-item" onclick="openLightbox(this)">
      <img src="/img/diploma/neyropsihologija.jpg" alt="Сертификат нейропсихолога" loading="lazy">
      <div class="diploma-title">Сертификат нейропсихолога</div>
    </div>
  </div>
</div>

<div id="lightbox" class="lightbox" onclick="closeLightbox()">
  <span class="close">&times;</span>
  <img id="lightbox-img" class="lightbox-content">
</div>

<script>
function openLightbox(element) {
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = document.getElementById("lightbox-img");
  lightboxImg.src = element.querySelector("img").src;
  lightbox.style.display = "block";
}

function closeLightbox() {
  document.getElementById("lightbox").style.display = "none";
}

// Close lightbox when pressing Escape key
document.addEventListener('keydown', function(event) {
  if (event.key === 'Escape') {
    closeLightbox();
  }
});
</script>

<div class="contact-section">
  <h2>Свяжитесь со мной</h2>
  <p>Если у вас есть вопросы или вы хотите записаться на консультацию, вы можете <a href="/contacts/">связаться со мной</a>.</p>
</div>

</div> 