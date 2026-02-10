<template>
  <footer class="footer">
    <div class="container">

      <div class="brand">
        <h2>DENTIST</h2>
        <p>
          Экспертная стоматология нового поколения.  
          Забота о здоровье и эстетике вашей улыбки.
        </p>
      </div>

      <div class="contacts">
        <div class="contact-item">
          <span class="label">Адрес</span>
          <p>г. Алматы, ул. Жолдасбекова 99</p>
        </div>

        <div class="contact-item">
          <span class="label">Телефон</span>
          <a href="tel:+77057733533">
            +7 705 773 35 33
          </a>
        </div>

        <div class="contact-item">
          <span class="label">Email</span>
          <a href="mailto:info@dentist.kz">
            info@dentist.kz
          </a>
        </div>

        <div class="socials">
          <a href="#">Instagram</a>
          <a href="#">WhatsApp</a>
        </div>

        <a href="#signup" class="cta">
          Записаться на консультацию
        </a>
      </div>

    </div>

    <!-- НИЗ -->
    <div class="bottom">
      © 2026 DENTIST. Все права защищены.
    </div>
  </footer>
</template>

<script setup lang="ts">
</script>

<style scoped>
.footer {
  background: #0b1320; /* глубокий дорогой цвет */
  color: #e5e7eb;
  padding-top: 70px;
}

/* контейнер */
.container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 32px;

  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 80px;
}

/* бренд */
.brand h2 {
  font-size: 30px;
  color: #ffffff;
  margin-bottom: 14px;
}

.brand p {
  line-height: 1.7;
  color: #9ca3af;
  max-width: 360px;
}

/* контакты */
.contacts {
  display: flex;
  flex-direction: column;
  gap: 18px;
}

.contact-item p,
.contact-item a {
  color: #e5e7eb;
  text-decoration: none;
  font-size: 16px;
}

.label {
  font-size: 13px;
  color: #6b7280;
  display: block;
  margin-bottom: 4px;
}

/* соцсети */
.socials {
  display: flex;
  gap: 18px;
  margin-top: 8px;
}

.socials a {
  color: #0f766e;
  font-weight: 600;
  text-decoration: none;
}

.socials a:hover {
  text-decoration: underline;
}

/* кнопка */
.cta {
  margin-top: 12px;
  background: #0f766e;
  padding: 14px;
  text-align: center;
  border-radius: 10px;
  color: white;
  text-decoration: none;
  font-weight: 700;
  transition: 0.25s;
}

.cta:hover {
  background: #115e59;
  transform: translateY(-2px);
}

/* низ */
.bottom {
  border-top: 1px solid #1f2937;
  margin-top: 60px;
  padding: 20px;
  text-align: center;
  font-size: 14px;
  color: #6b7280;
}

/* 📱 адаптив */
@media (max-width: 768px) {
  .container {
    grid-template-columns: 1fr;
    gap: 40px;
  }
}
</style>
