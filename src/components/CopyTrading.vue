<template>
  <div class="page-section copy-trading mb-4" id="copy-trading">
    <div class="container">
      <div class="row justify-content-center text-center wow fadeInUp">
        <div class="col-lg-6">
          <h5 class="mb-3 ct-text">Copy Trading</h5>
          <h1 class="mb-3">Trading becomes Investment</h1>
          <p class="mb-5">Connect your investment with top strategy traders through Copy2trade</p>
        </div>
      </div>
      <div class="pricing-table mobile-preview img-place floating-animate copy-img">
        <img
          src="https://dynamic-images.admiralmarkets.com/1392x,webp/static-images.admiralmarkets.com/data/homepage/go_beyond_trading/hero.png  "
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<script setup>
import { onMounted } from 'vue'
import AOS from 'aos'

onMounted(() => {
  AOS.init()
})
</script>

<style>
.ct-gap {
  height: 25px;
  background-color: black;
}
.copy-trading {
  background-image: url('../assets/img/bg_hero_2.svg');
  height: 100vh;
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}
.copy-img {
  width: 50%;
}

.ct-text {
  text-shadow: -15px 5px 20px #000000;
}

@media screen and (max-width: 768px) {
  .copy-img {
    width: 100%;
  }
}
</style>
