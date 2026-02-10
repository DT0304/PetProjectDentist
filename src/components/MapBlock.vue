<template>
  <section class="map-section" id="map">
    <div class="container">
      <header class="head">
        <h2 class="title">Как нас найти</h2>
        <p class="subtitle">
          Мы находимся в удобной локации — легко добраться и припарковаться.
        </p>
      </header>
    </div>

    <!-- ЯНДЕКС КАРТА -->
    <div ref="mapEl" class="map"></div>
  </section>
</template>

<script setup lang="ts">
import { onMounted, ref } from 'vue'

const mapEl = ref<HTMLDivElement | null>(null)

// координаты клиники (Алматы)
const coords: [number, number] = [43.232884, 76.951297]

onMounted(() => {
  // если API уже загружен — просто инициализируем
  if ((window as any).ymaps) {
    initMap()
    return
  }

  // динамически подключаем Яндекс API
  const script = document.createElement('script')
  script.src = 'https://api-maps.yandex.ru/2.1/?lang=ru_RU'
  script.async = true
  script.onload = initMap
  document.head.appendChild(script)
})

function initMap() {
  const ymaps = (window as any).ymaps
  if (!ymaps || !mapEl.value) return

  ymaps.ready(() => {
    const map = new ymaps.Map(mapEl.value, {
      center: coords,
      zoom: 15,
      controls: ['zoomControl', 'fullscreenControl'],
    })

    map.behaviors.disable('scrollZoom')

    // маркер клиники
    const placemark = new ymaps.Placemark(
      coords,
      {
        balloonContent: '<strong>DENTIST</strong><br/>Стоматологическая клиника',
      },
      {
        preset: 'islands#redIcon',
      }
    )

    map.geoObjects.add(placemark)
  })
}
</script>

<style scoped>
.map-section {
  padding: 80px 0 80px;
  background: #ffffff;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 32px;
}

.head {
  margin-bottom: 24px;
}

.title {
  font-size: 36px;
  font-weight: 900;
  color: #111827;
  margin: 0 0 10px;
}

.subtitle {
  font-size: 15px;
  line-height: 1.7;
  color: #374151;
  max-width: 520px;
}

/* карта */
.map {
  width: 100%;
  height: 520px;
  border-radius: 24px 24px 0 0;
  overflow: hidden;
  box-shadow: 0 -20px 40px rgba(0, 0, 0, 0.12);
}

/* mobile */
@media (max-width: 640px) {
  .container {
    padding: 0 16px;
  }

  .map {
    height: 380px;
    border-radius: 16px 16px 0 0;
  }
}
</style>