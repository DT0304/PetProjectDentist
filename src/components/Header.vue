<template>
  <header class="header">
    <!-- LOGO -->
    <div class="dent-logo">
      <span>DENTIST</span>
    </div>

    <!-- MENU -->
    <nav class="dent-menu">
      <ul>
        <li><a href="#home">Главная</a></li>
        <li><a href="#services">Услуги</a></li>
        <li><a href="#doctors">Врачи</a></li>
        <li><a href="#reviews">Отзывы</a></li>
      </ul>
    </nav>

    <!-- CONTACTS -->
    <div class="dent-contact">
      <div class="dent-address">
        <span class="label">Адрес:</span>
        <span>г. Алматы</span>
      </div>

      <div class="dent-social">
        <a href="#" aria-label="WhatsApp"><img src="../../public/whatsapp.svg" alt="wp-icon" class="cn-logo"></a>
        <a href="#" aria-label="Instagram"><img src="../../public/instagram.svg" alt="inst-icon" class="cn-logo"></a>
      </div>

      <div class="dent-tel">
        <span class="label">Контакты:</span>
        <a href="tel:+77057733533">+7 705 773 35 33</a>
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">

</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 32px;
  background: #ffffff;
  border-bottom: 1px solid #e5e7eb;
}
.cn-logo {
  width: 2.5rem;
  height: 2.5rem;
  display: block;
}
/* LOGO */
.dent-logo {
  font-size: 20px;
  font-weight: 700;
  color: #0f766e;
}

/* MENU */
.dent-menu ul {
  display: flex;
  gap: 24px;
  list-style: none;
  padding: 0;
  margin: 0;
}

.dent-menu a {
  text-decoration: none;
  color: #111827;
  font-weight: 500;
}

.dent-menu a:hover {
  color: #0f766e;
}

/* CONTACTS */
.dent-contact {
  display: flex;
  align-items: center;
  gap: 24px;
  font-size: 14px;
}

.label {
  font-weight: 600;
  margin-right: 4px;
}

.dent-social {
    display: flex;
}

.dent-social a {
  margin-right: 12px;
  text-decoration: none;
  color: #0f766e;
}

.dent-social a:hover {
  text-decoration: underline;
}

.dent-tel a {
  text-decoration: none;
  color: #111827;
  font-weight: 600;
}
</style>