<script setup>
import IMG_COUPON_MIDDLE from '@/assets/coupon_card_middle.svg'
import IMG_ORDER from '@/assets/empty_order.svg'
</script>

<template>
  <main>
    <div class="grid-container">
      <div class="grid-item">
        <p>CSS - backgroundImage - SVG 1</p>
        <div class="img-box" :style="{ backgroundImage: `url(${IMG_COUPON_MIDDLE})` }"></div>
      </div>
      <div class="grid-item">
        <p>CSS - backgroundImage - SVG 2</p>
        <div class="img-box" :style="{ backgroundImage: `url(${IMG_ORDER})` }"></div>
      </div>
      <div class="grid-item">
        <p>style - backgroundImage - SVG 1</p>
        <div class="img-box img-1"></div>
      </div>
      <div class="grid-item">
        <p>style - backgroundImage - SVG 2</p>
        <div class="img-box img-2"></div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.grid-container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, auto);
  gap: 10px;
}

p {
  font-size: 20px;
  font-weight: 600;
}

.img-box {
  width: 300px;
  height: 200px;
  background-repeat: no-repeat;
  background-size: contain;
}

.img-1 {
  background-image: url("@/assets/coupon_card_middle.svg");
}

.img-2 {
  background-image: url("@/assets/empty_order.svg");
}
</style>
