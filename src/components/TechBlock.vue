<template>
  <section class="tech-showcase" id="tech">
    <div class="container">
      <!-- Верх -->
      <header class="hero">
        <div class="hero-left">
          <p class="kicker">ТЕХНОЛОГИИ</p>
          <h2 class="title">
            Цифровая стоматология <span>DENTIST</span> —
            точность, комфорт, предсказуемый результат
          </h2>
          <p class="subtitle">
            Мы используем современное оборудование и протоколы, чтобы лечение было максимально
            аккуратным, безопасным и понятным для пациента.
          </p>

          <div class="badges">
            <span class="badge">3D-диагностика</span>
            <span class="badge">Цифровое планирование</span>
            <span class="badge">Стерильность</span>
            <span class="badge">Комфорт</span>
          </div>

          <div class="cta">
            <a class="btn primary" href="#signup">Записаться</a>
            <a class="btn ghost" href="#services">Смотреть услуги</a>
          </div>
        </div>

        <div class="hero-right">
          <div class="panel">
            <div class="panel-top">
              <div class="dot"></div>
              <div class="dot"></div>
              <div class="dot"></div>
            </div>

            <div class="panel-body">
              <div class="metric">
                <div class="metric-num">01</div>
                <div class="metric-text">
                  <strong>План лечения</strong>
                  <span>по шагам и без “сюрпризов”</span>
                </div>
              </div>

              <div class="metric">
                <div class="metric-num">02</div>
                <div class="metric-text">
                  <strong>Контроль качества</strong>
                  <span>на каждом этапе</span>
                </div>
              </div>

              <div class="metric">
                <div class="metric-num">03</div>
                <div class="metric-text">
                  <strong>Комфорт пациента</strong>
                  <span>бережные протоколы</span>
                </div>
              </div>

              <div class="divider"></div>

              <div class="line">
                <span class="chip">Точность</span>
                <span class="chip">Безопасность</span>
                <span class="chip">Эстетика</span>
              </div>
            </div>
          </div>
        </div>
      </header>

      <!-- Низ: креативная “лента” технологий -->
      <div class="tracks">
        <div class="track">
          <div class="track-title">
            <span class="track-icon">🔎</span>
            <h3>Диагностика</h3>
          </div>
          <div class="track-cards">
            <div class="tcard">
              <strong>3D-снимки и оценка</strong>
              <p>Понимаем картину целиком и выбираем правильную тактику.</p>
            </div>
            <div class="tcard">
              <strong>Фотопротокол</strong>
              <p>Фиксируем “до/после” и контролируем детали лечения.</p>
            </div>
            <div class="tcard">
              <strong>План на понятном языке</strong>
              <p>Сроки, этапы, рекомендации — без сложных терминов.</p>
            </div>
          </div>
        </div>

        <div class="track">
          <div class="track-title">
            <span class="track-icon">🧠</span>
            <h3>Цифровые протоколы</h3>
          </div>
          <div class="track-cards">
            <div class="tcard">
              <strong>3D-планирование</strong>
              <p>Прорабатываем этапы заранее — результат становится предсказуемым.</p>
            </div>
            <div class="tcard">
              <strong>Командный подход</strong>
              <p>Единый протокол — одинаково высокий стандарт у всей команды.</p>
            </div>
            <div class="tcard">
              <strong>Контроль на этапах</strong>
              <p>Проверяем качество “по чек-листу”, а не “на глаз”.</p>
            </div>
          </div>
        </div>

        <div class="track">
          <div class="track-title">
            <span class="track-icon">🎯</span>
            <h3>Точность и эстетика</h3>
          </div>
          <div class="track-cards">
            <div class="tcard">
              <strong>Микроточность</strong>
              <p>Бережём ткани зуба и работаем максимально аккуратно.</p>
            </div>
            <div class="tcard">
              <strong>Естественный дизайн улыбки</strong>
              <p>Гармония формы и цвета — без “перебора”.</p>
            </div>
            <div class="tcard">
              <strong>Долговечные материалы</strong>
              <p>Подбираем решение под задачу: красиво и надолго.</p>
            </div>
          </div>
        </div>

        <div class="track">
          <div class="track-title">
            <span class="track-icon">🧼</span>
            <h3>Безопасность и комфорт</h3>
          </div>
          <div class="track-cards">
            <div class="tcard">
              <strong>Стерильность как стандарт</strong>
              <p>Чистота инструментов и кабинетов — приоритет №1.</p>
            </div>
            <div class="tcard">
              <strong>Комфортное обезболивание</strong>
              <p>Лечение без лишнего стресса и напряжения.</p>
            </div>
            <div class="tcard">
              <strong>Забота о пациентах</strong>
              <p>Поддержка и объяснения до, во время и после процедур.</p>
            </div>
          </div>
        </div>
      </div>

      <!-- Финальный слоган -->
      <div class="final">
        <div class="final-left">
          <p class="final-kicker">НАША ФИЛОСОФИЯ</p>
          <h3 class="final-title">Технологии, которые работают на вашу улыбку</h3>
          <p class="final-sub">
            Мы выбираем решения, которые дают уверенность: точность, безопасность и прогнозируемый результат.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
</script>

<style scoped>
.tech-showcase {
  padding: 90px 0;
  background:
    radial-gradient(900px 500px at 15% 15%, rgba(15, 118, 110, 0.14), transparent 55%),
    radial-gradient(900px 500px at 85% 20%, rgba(17, 94, 89, 0.10), transparent 55%),
    #ffffff;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 32px;
}

/* HERO */
.hero {
  display: grid;
  grid-template-columns: 1.15fr 0.85fr;
  gap: 28px;
  align-items: stretch;
  margin-bottom: 26px;
}

.kicker {
  margin: 0 0 10px;
  font-size: 12px;
  font-weight: 800;
  letter-spacing: 2px;
  color: #0f766e;
}

.title {
  margin: 0 0 12px;
  font-size: 42px;
  line-height: 1.1;
  font-weight: 900;
  letter-spacing: -0.6px;
  color: #111827;
}

.title span {
  color: #0f766e;
}

.subtitle {
  margin: 0 0 16px;
  font-size: 16px;
  line-height: 1.75;
  color: #374151;
  max-width: 680px;
}

.badges {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin: 14px 0 18px;
}

.badge {
  padding: 8px 12px;
  border-radius: 999px;
  border: 1px solid rgba(15, 118, 110, 0.22);
  background: rgba(255, 255, 255, 0.65);
  font-size: 12px;
  font-weight: 800;
  color: #0f766e;
  backdrop-filter: blur(6px);
}

.cta {
  display: flex;
  gap: 10px;
  margin-top: 10px;
}

/* PANEL справа */
.panel {
  border-radius: 18px;
  border: 1px solid #e5e7eb;
  background: rgba(255, 255, 255, 0.75);
  box-shadow: 0 22px 50px rgba(0, 0, 0, 0.08);
  overflow: hidden;
  backdrop-filter: blur(8px);
  height: 100%;
}

.panel-top {
  display: flex;
  gap: 8px;
  padding: 12px 14px;
  border-bottom: 1px solid #eef2f7;
  background: rgba(15, 118, 110, 0.04);
}

.dot {
  width: 10px;
  height: 10px;
  border-radius: 999px;
  background: rgba(15, 118, 110, 0.35);
}

.panel-body {
  padding: 16px;
}

.metric {
  display: grid;
  grid-template-columns: 52px 1fr;
  gap: 12px;
  padding: 12px;
  border-radius: 14px;
  border: 1px solid #eef2f7;
  background: rgba(255, 255, 255, 0.9);
  margin-bottom: 10px;
}

.metric-num {
  font-weight: 900;
  color: #0f766e;
  font-size: 18px;
  display: grid;
  place-items: center;
  border-radius: 12px;
  background: rgba(15, 118, 110, 0.10);
}

.metric-text strong {
  display: block;
  color: #111827;
  font-weight: 900;
  margin-bottom: 2px;
}

.metric-text span {
  color: #374151;
  font-size: 13px;
}

.divider {
  height: 1px;
  background: #eef2f7;
  margin: 14px 0;
}

.line {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.chip {
  font-size: 12px;
  font-weight: 900;
  color: #111827;
  padding: 8px 10px;
  border-radius: 999px;
  background: rgba(17, 24, 39, 0.05);
  border: 1px solid #eef2f7;
}

/* TRACKS */
.tracks {
  display: grid;
  gap: 14px;
}

.track {
  border-radius: 18px;
  border: 1px solid #e5e7eb;
  background: rgba(255, 255, 255, 0.85);
  box-shadow: 0 16px 40px rgba(0, 0, 0, 0.06);
  overflow: hidden;
}

.track-title {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 16px 18px;
  border-bottom: 1px solid #eef2f7;
  background: rgba(15, 118, 110, 0.04);
}

.track-title h3 {
  margin: 0;
  font-size: 16px;
  font-weight: 900;
  color: #111827;
}

.track-icon {
  width: 34px;
  height: 34px;
  border-radius: 12px;
  background: rgba(15, 118, 110, 0.10);
  display: grid;
  place-items: center;
  font-size: 16px;
}

.track-cards {
  padding: 16px 18px 18px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
}

.tcard {
  border-radius: 16px;
  border: 1px solid #eef2f7;
  background: #ffffff;
  padding: 14px;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.tcard:hover {
  transform: translateY(-3px);
  box-shadow: 0 18px 40px rgba(0, 0, 0, 0.08);
}

.tcard strong {
  display: block;
  font-size: 14px;
  font-weight: 900;
  color: #111827;
  margin-bottom: 6px;
}

.tcard p {
  margin: 0;
  font-size: 13px;
  line-height: 1.6;
  color: #374151;
}

/* FINAL */
.final {
  margin-top: 18px;
  border-radius: 18px;
  border: 1px solid rgba(15, 118, 110, 0.22);
  background: rgba(15, 118, 110, 0.06);
  padding: 18px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  gap: 16px;
}

.final-kicker {
  margin: 0 0 6px;
  font-size: 12px;
  font-weight: 900;
  letter-spacing: 2px;
  color: #0f766e;
}

.final-title {
  margin: 0 0 6px;
  font-size: 20px;
  font-weight: 900;
  color: #111827;
}

.final-sub {
  margin: 0;
  font-size: 14px;
  line-height: 1.6;
  color: #374151;
}

/* BUTTONS */
.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 12px 16px;
  border-radius: 12px;
  font-size: 14px;
  font-weight: 900;
  text-decoration: none;
  cursor: pointer;
  transition: transform 0.2s ease, background 0.2s ease, border-color 0.2s ease;
  border: 1px solid transparent;
  user-select: none;
  white-space: nowrap;
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
  background: rgba(255, 255, 255, 0.8);
  color: #0f766e;
  border-color: rgba(15, 118, 110, 0.25);
}

.ghost:hover {
  border-color: #0f766e;
}

/* RESPONSIVE */
@media (max-width: 980px) {
  .hero {
    grid-template-columns: 1fr;
  }
  .title {
    font-size: 34px;
  }
  .track-cards {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 640px) {
  .container {
    padding: 0 16px;
  }
  .final {
    flex-direction: column;
    align-items: stretch;
  }
}
</style>
