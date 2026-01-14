<template>
  <section class="team-photo" id="home">
    <!-- ФОН -->
    <img
      src="../../public/BackgroundPhoto.png"
      alt="Команда стоматологии"
      class="bg-image"
    />

    <!-- ПОЛУПРОЗРАЧНЫЙ БЛОК -->
    <div class="sign-block">
      <span class="brand">DENTIST</span>
      <span class="title">Экспертная стоматология</span>
      <span class="subtitle">нового поколения</span>

      <button class="sign-btn">
        Записаться на консультацию
      </button>
    </div>
  </section>
</template>

<script setup lang="ts">
</script>

<style scoped>
/* ОБЩИЙ КОНТЕЙНЕР */
.team-photo {
  position: relative;
  width: 100%;
  height: 650px; /* можно менять */
  overflow: hidden;
}

/* ФОНОВОЕ ИЗОБРАЖЕНИЕ */
.bg-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center 5%;
}

/* БЕЛЫЙ ПОЛУПРОЗРАЧНЫЙ БЛОК */
.sign-block {
  position: absolute;
  top: 75%;              /* чуть ниже центра */
  left: 50%;
  transform: translate(-50%, -50%);

  background: rgba(255, 255, 255, 0.9); /* 5–10% прозрачности */
  padding: 40px 48px;
  text-align: center;

  border-radius: 12px;
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);

  max-width: 520px;
  width: 90%;
}

/* ТЕКСТ */
.brand {
  font-size: 14px;
  letter-spacing: 2px;
  font-weight: 600;
  color: #0f766e;
  display: block;
  margin-bottom: 8px;
}

.title {
  font-size: 28px;
  font-weight: 700;
  color: #111827;
  display: block;
}

.subtitle {
  font-size: 20px;
  font-weight: 500;
  color: #374151;
  margin-bottom: 24px;
  display: block;
}

/* КНОПКА */
.sign-btn {
  background: #0f766e;
  color: #ffffff;
  border: none;
  padding: 14px 28px;
  font-size: 14px;
  font-weight: 600;
  letter-spacing: 1px;
  border-radius: 8px;
  cursor: pointer;
  transition: all 0.25s ease;
}

.sign-btn:hover {
  background: #115e59;
  transform: translateY(-2px);
}
</style>
