<template>
  <section class="faq" id="faq">
    <div class="container">
      <header class="head">
        <h2 class="title">FAQ</h2>
        <p class="subtitle">Коротко отвечаем на самые частые вопросы.</p>
      </header>

      <div class="list" role="list">
        <details v-for="(item, i) in items" :key="i" class="q">
          <summary class="q-head">
            <span class="q-title">{{ item.q }}</span>
            <span class="q-icon" aria-hidden="true">+</span>
          </summary>

          <div class="q-body">
            <p>{{ item.a }}</p>
          </div>
        </details>
      </div>

      <div class="note">
        Не нашли ответ? <a href="#signup">Напишите нам</a> — подскажем и поможем записаться.
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
type FaqItem = { q: string; a: string }

const items: FaqItem[] = [
  {
    q: "Сколько длится консультация?",
    a: "Обычно 20–40 минут: осмотр, рекомендации и план лечения по этапам.",
  },
  {
    q: "Больно ли лечить зубы?",
    a: "Мы используем современное обезболивание и бережные протоколы — лечение проходит комфортно.",
  },
  {
    q: "Можно ли записаться в тот же день?",
    a: "Если есть свободное окно — да. Оставьте заявку, и мы предложим ближайшее время.",
  },
  {
    q: "Какие способы оплаты доступны?",
    a: "Наличные и безналичный расчёт. Уточните детали при записи — подскажем удобный вариант.",
  },
]
</script>

<style scoped>
.faq {
  padding: 0px 0 60px;
  background: #ffffff;
}

.container {
  max-width: 900px;
  margin: 0 auto;
  padding: 0 32px;
}

.head {
  margin-bottom: 22px;
}

.title {
  margin: 0 0 10px;
  font-size: 38px;
  font-weight: 900;
  letter-spacing: -0.5px;
  color: #111827;
}

.subtitle {
  margin: 0;
  font-size: 15px;
  line-height: 1.7;
  color: #374151;
}

/* FAQ list */
.list {
  display: grid;
  gap: 10px;
}

.q {
  border: 1px solid #e5e7eb;
  border-radius: 16px;
  background: rgba(255, 255, 255, 0.85);
  box-shadow: 0 14px 30px rgba(0, 0, 0, 0.05);
  overflow: hidden;
}

/* summary */
.q-head {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 14px;
  padding: 16px 16px;
  cursor: pointer;
  user-select: none;
}

.q-head::-webkit-details-marker {
  display: none;
}

.q-title {
  font-size: 15px;
  font-weight: 800;
  color: #111827;
}

.q-icon {
  width: 34px;
  height: 34px;
  border-radius: 12px;
  display: grid;
  place-items: center;
  font-size: 18px;
  font-weight: 900;
  color: #0f766e;
  background: rgba(15, 118, 110, 0.10);
  transition: transform 0.2s ease;
}

/* content */
.q-body {
  padding: 0 16px 16px;
}

.q-body p {
  margin: 0;
  font-size: 14px;
  line-height: 1.7;
  color: #374151;
}

/* open state */
.q[open] .q-icon {
  transform: rotate(45deg);
}

/* note */
.note {
  margin-top: 16px;
  font-size: 14px;
  color: #374151;
}

.note a {
  color: #0f766e;
  font-weight: 800;
  text-decoration: none;
}

.note a:hover {
  text-decoration: underline;
}

/* responsive */
@media (max-width: 640px) {
  .container {
    padding: 0 16px;
  }
  .title {
    font-size: 30px;
  }
}
</style>