---
layout: service
title: Занятия в кабинете
images:
  - src: /img/cabinet/cabinet1.jpg
    alt: Кабинет 1
  - src: /img/cabinet/cabinet2.jpg
    alt: Кабинет 2
  - src: /img/cabinet/cabinet3.jpg
    alt: Кабинет 3
  - src: /img/cabinet/cabinet4.jpg
    alt: Кабинет 4
  - src: /img/cabinet/cabinet5.jpg
    alt: Кабинет 5
  - src: /img/cabinet/cabinet6.jpg
    alt: Кабинет 6
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

.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 0.5rem;
  margin: 2rem 0;
  max-width: 800px;
  margin-left: auto;
  margin-right: auto;
}

.gallery-item {
  position: relative;
  overflow: hidden;
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
  cursor: pointer;
  aspect-ratio: 1;
}

.gallery-item:hover {
  transform: scale(1.05);
}

.gallery-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
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

@media (max-width: 768px) {
  .gallery {
    grid-template-columns: repeat(2, 1fr);
    gap: 0.3rem;
  }
}
</style>

<div class="consultation-container">
<h1 class="page-title">Кабинет</h1>

Я принимаю на консультации и занятия с детьми в своем кабинете состоящем из 2 комнат в Риге. 

<div class="gallery">
  {% for image in page.images %}
  <div class="gallery-item" onclick="openLightbox(this)">
    <img src="{{ image.src }}" alt="{{ image.alt }}">
  </div>
  {% endfor %}
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

(информация дополняется)
</div>