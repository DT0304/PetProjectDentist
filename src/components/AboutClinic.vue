<template>
  <section class="about" id="about">
    <!-- ЛЕВАЯ ЧАСТЬ: ТЕКСТ -->
    <div class="about-content">
      <h2 class="about-title">
        Экспертная стоматология <span>DENTIST</span>
      </h2>

      <p class="about-text">
        DENTIST — это современная стоматологическая клиника, где сочетаются
        передовые технологии, клинический опыт и забота о пациенте.
        Мы подходим к лечению комплексно, уделяя внимание не только эстетике,
        но и функциональному здоровью улыбки.
      </p>

      <p class="about-text">
        Наша команда — это специалисты нового поколения, которые постоянно
        развиваются, внедряют инновационные методики и создают комфортную,
        доверительную атмосферу для каждого пациента.
      </p>

      <!-- СЛОГАН -->
      <div class="about-slogan">
        Мы создаём улыбки, которые работают на ваше будущее
      </div>
    </div>

    <!-- ПРАВАЯ ЧАСТЬ: ФОТО -->
    <div class="about-team">
      <img src="../../public/team.png" alt="Команда стоматологии DENTIST">
    </div>
  </section>
</template>

<script setup lang="ts">
</script>

<style scoped>
.about {
  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  gap: 48px;
  align-items: center;

  padding: 80px 32px;
  max-width: 1200px;
  margin: 0 auto;
}

/* ЛЕВАЯ ЧАСТЬ */
.about-content {
  display: flex;
  flex-direction: column;
}

.about-title {
  font-size: 36px;
  font-weight: 700;
  color: #111827;
  margin-bottom: 24px;
}

.about-title span {
  color: #0f766e;
}

.about-text {
  font-size: 16px;
  line-height: 1.7;
  color: #374151;
  margin-bottom: 16px;
}

/* СЛОГАН */
.about-slogan {
  margin-top: 32px;
  padding-left: 16px;
  border-left: 4px solid #0f766e;

  font-size: 20px;
  font-weight: 600;
  color: #0f766e;
}

/* ПРАВАЯ ЧАСТЬ */
.about-team img {
  width: 100%;
  border-radius: 16px;
  object-fit: cover;
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
}

/* АДАПТИВ */
@media (max-width: 900px) {
  .about {
    grid-template-columns: 1fr;
  }

  .about-team {
    order: -1;
  }
}
</style>
