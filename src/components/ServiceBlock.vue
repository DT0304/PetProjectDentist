<template>
  <section class="services" id="services">
    <div class="container">
      <header class="head">
        <h2 class="title">Услуги клиники <span>DENTIST</span></h2>
        <p class="subtitle">
          От профилактики до сложных случаев — всё в одном месте, с понятным планом лечения и заботой о вашем комфорте.
        </p>
      </header>

      <div class="grid">
        <article
          v-for="item in services"
          :key="item.title"
          class="card"
        >
          <div class="card-top">
            <div class="icon" aria-hidden="true">
              {{ item.icon }}
            </div>

            <div class="card-title">
              <h3>{{ item.title }}</h3>
              <p class="tag">{{ item.level }}</p>
            </div>
          </div>

          <p class="desc">{{ item.desc }}</p>

          <ul class="list">
            <li v-for="point in item.points" :key="point">
              <span class="dot" aria-hidden="true"></span>
              <span>{{ point }}</span>
            </li>
          </ul>

          <div class="actions">
            <a class="btn primary" href="#signup">Записаться</a>
            <a class="btn ghost" href="#prices">Цены</a>
          </div>
        </article>
      </div>

      <div class="bottom">
        <div class="note">
          <strong>Не знаете, что выбрать?</strong>
          Оставьте заявку — мы подскажем услугу и составим план лечения после консультации.
        </div>
        <a class="btn primary big" href="#signup">Записаться на консультацию</a>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
type Service = {
  icon: string
  title: string
  level: string
  desc: string
  points: string[]
}

const services: Service[] = [
  {
    icon: "🛡️",
    title: "Профилактика и гигиена",
    level: "Базовый уровень",
    desc:
      "Здоровая улыбка начинается с регулярного ухода. Делаем профилактику комфортно и бережно.",
    points: [
      "Профессиональная чистка и полировка",
      "AirFlow и удаление налёта/камня",
      "Фторирование и реминерализация",
      "Индивидуальные рекомендации по уходу",
    ],
  },
  {
    icon: "✨",
    title: "Эстетическая стоматология",
    level: "Эстетика",
    desc:
      "Подчеркнём естественную красоту улыбки — аккуратно, без перегруза и «искусственности».",
    points: [
      "Отбеливание и устранение пигментации",
      "Реставрации и художественная коррекция",
      "Виниры и эстетические решения",
      "Дизайн улыбки (подбор формы/тона)",
    ],
  },
  {
    icon: "🦷",
    title: "Терапевтическое лечение",
    level: "Средняя сложность",
    desc:
      "Лечим кариес и сохраняем зубы. Приоритет — точность, безопасность и долговечный результат.",
    points: [
      "Лечение кариеса и пломбирование",
      "Лечение каналов (эндодонтия)",
      "Повторное лечение и сложные случаи",
      "Диагностика и снимки по показаниям",
    ],
  },
  {
    icon: "🧩",
    title: "Ортодонтия",
    level: "Долгосрочный результат",
    desc:
      "Исправление прикуса и выравнивание зубов — с прозрачным планом и регулярным контролем.",
    points: [
      "Брекеты и элайнеры",
      "Коррекция прикуса у взрослых и подростков",
      "Ретенция (закрепление результата)",
      "Планирование сроков и этапов лечения",
    ],
  },
  {
    icon: "🦴",
    title: "Хирургия и имплантация",
    level: "Высокая сложность",
    desc:
      "Когда нужно серьёзное решение: удаление, подготовка и восстановление зубов с опорой на импланты.",
    points: [
      "Удаление зубов (в т.ч. сложное)",
      "Имплантация и восстановление зубов",
      "Подготовка к имплантации (по показаниям)",
      "Сопровождение и контроль заживления",
    ],
  },
  {
    icon: "👑",
    title: "Ортопедия и протезирование",
    level: "Премиум-решения",
    desc:
      "Возвращаем комфорт жевания и эстетику: коронки, мосты и комплексные протоколы восстановления.",
    points: [
      "Коронки и вкладки (восстановление формы)",
      "Мостовидные протезы",
      "Полное восстановление улыбки",
      "Подбор материалов под задачу и бюджет",
    ],
  },
]
</script>

<style scoped>
.services {
  padding: 50px 0;
  background: #ffffff;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 32px;
}

.head {
  max-width: 760px;
  margin-bottom: 36px;
}

.title {
  font-size: 40px;
  font-weight: 800;
  color: #111827;
  letter-spacing: -0.5px;
  margin: 0 0 12px 0;
}

.title span {
  color: #0f766e;
}

.subtitle {
  margin: 0;
  font-size: 16px;
  line-height: 1.7;
  color: #374151;
}

.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 18px;
}

.card {
  border: 1px solid #e5e7eb;
  border-radius: 16px;
  padding: 18px 18px 16px;
  background: #fff;
  box-shadow: 0 14px 28px rgba(0, 0, 0, 0.06);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  min-height: 320px;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 18px 38px rgba(0, 0, 0, 0.10);
}

.card-top {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 10px;
}

.icon {
  width: 44px;
  height: 44px;
  border-radius: 12px;
  background: rgba(15, 118, 110, 0.10);
  display: grid;
  place-items: center;
  font-size: 20px;
}

.card-title h3 {
  margin: 0;
  font-size: 18px;
  font-weight: 800;
  color: #111827;
}

.tag {
  margin: 4px 0 0 0;
  font-size: 12px;
  font-weight: 600;
  color: #0f766e;
}

.desc {
  margin: 10px 0 12px;
  font-size: 14px;
  line-height: 1.7;
  color: #374151;
}

.list {
  list-style: none;
  padding: 0;
  margin: 0 0 16px 0;
  display: grid;
  gap: 8px;
}

.list li {
  display: flex;
  gap: 10px;
  align-items: flex-start;
  color: #111827;
  font-size: 13px;
  line-height: 1.5;
}

.dot {
  width: 8px;
  height: 8px;
  margin-top: 6px;
  border-radius: 999px;
  background: #0f766e;
  flex: 0 0 8px;
}

.actions {
  display: flex;
  gap: 10px;
  margin-top: auto;
}

.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 10px 14px;
  border-radius: 10px;
  font-size: 13px;
  font-weight: 700;
  text-decoration: none;
  cursor: pointer;
  transition: transform 0.2s ease, background 0.2s ease, border-color 0.2s ease;
  user-select: none;
  border: 1px solid transparent;
}

.btn:active {
  transform: translateY(1px);
}

.primary {
  background: #0f766e;
  color: #fff;
}

.primary:hover {
  background: #115e59;
}

.ghost {
  background: #fff;
  color: #0f766e;
  border-color: #cbd5e1;
}

.ghost:hover {
  border-color: #0f766e;
}

.bottom {
  margin-top: 28px;
  padding: 18px;
  border: 1px solid #e5e7eb;
  border-radius: 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
  background: rgba(15, 118, 110, 0.04);
}

.note {
  color: #111827;
  font-size: 14px;
  line-height: 1.6;
}

.big {
  padding: 12px 18px;
  font-size: 14px;
}

/* Адаптив */
@media (max-width: 980px) {
  .grid {
    grid-template-columns: repeat(2, 1fr);
  }
  .title {
    font-size: 34px;
  }
}

@media (max-width: 640px) {
  .container {
    padding: 0 16px;
  }
  .grid {
    grid-template-columns: 1fr;
  }
  .bottom {
    flex-direction: column;
    align-items: stretch;
  }
  .title {
    font-size: 30px;
  }
}
</style>