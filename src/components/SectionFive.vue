<template>
  <div class="section-five text-start pb-4" id="section-three">
    <div style="max-width: 1500px">
      <h1 class="section-five-heading">What is your choice of trading account?</h1>
      <div class="row section-five-card">
        <div data-aos="fade-up" class="col card-first">
          <img src="../assets/img/phone.png" alt="" class="section-five-img" />
          <div class="inner-text">0.6P</div>
          <h2 class="section-five-text">Low Spread</h2>
          <a class="text-decoration-none" href="https://b2pip.com/trading-account" target="_blank">
            <h5 class="learn-more mt-4">Learn More</h5>
          </a>
        </div>

        <div data-aos="fade-up" data-aos-delay="200" class="col card-second">
          <img src="../assets/img/earth.png" alt="" class="section-five-img" />
          <div class="inner-text">6$ per lakh</div>
          <h2 class="section-five-text">Zero Spread</h2>
          <a class="text-decoration-none" href="https://b2pip.com/trading-account" target="_blank">
            <h5 class="learn-more mt-4">Learn More</h5>
          </a>
        </div>
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
@media (min-width: 800px) and (max-width: 1200px) {
  .section-five-text {
    font:
      14px/20px 'Inter',
      sans-serif;
    font-weight: 600;
    letter-spacing: 4px;
    text-transform: uppercase;
  }
}
.section-five-img {
  width: 90%;
  margin-top: 1em;
  margin-bottom: 1em;
  border-radius: 25px;
  box-shadow: 0 0 10px #c9f73a;
}
.card-second,
.section-five-card {
  margin-left: 14%;
}
.card-second {
  margin-top: 3%;
  margin-left: 0 !important;
  margin-right: 11%;
}

.card-second .inner-text {
  /* position: absolute; */
  left: 37%;
  font-size: 25px;
  font-weight: 600;
  top: 39%;
}
.card-first .inner-text {
  /* position: absolute; */
  left: 47%;
  font-size: 25px;
  font-weight: 600;
  top: 29%;
}
.learn-more::after {
  content: '';
  display: inline-block;
  margin-left: 12px;
  vertical-align: middle;
  width: 37px;
  height: 17px;
  background-image: url("data:image/svg+xml,%3Csvg width='37' height='17' viewBox='0 0 37 17' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cline x1='-4.37114e-08' y1='8.5' x2='36' y2='8.5' stroke='black'/%3E%3Cpath d='M29 1L36 8.5L29 16' stroke='black'/%3E%3C/svg%3E%0A");
}
.learn-more {
  font:
    16px/24px 'Inter',
    sans-serif;
  font-weight: 400;
  text-decoration: none;
  color: #000;
  margin-top: 8px;
}
.section-five-heading {
  font-family: 'Nekst', sans-serif;
  font-size: 57px;
  font-weight: 600;
  width: 51%;
  margin-left: 11rem;
  margin-top: 5rem;
  margin-bottom: 5rem;
}
@media (max-width: 1100px) {
  .section-five-heading {
    margin-left: 0;
    width: auto;
  }
  .inner-text {
    font-size: 16px !important;
  }
}

@media (max-width: 800px) {
  .card-first {
    min-width: 70%;
  }
  .section-five-text {
    font:
      20px/30px 'Inter',
      sans-serif;
    font-weight: 600;
    letter-spacing: 5px;
    text-transform: uppercase;
    margin-top: 16px;
  }
  .card-second,
  .section-five-card {
    margin: auto;
  }
}
.section-five {
  width: 85vw;
  margin: auto;
  justify-content: center;
  display: flex;
}

.section-five-text {
  font:
    20px/30px 'Inter',
    sans-serif;
  font-weight: 600;
  letter-spacing: 5px;
  text-transform: uppercase;
}

@media (min-width: 2000px) {
  .card-second {
    margin-right: 5%;
  }
}
</style>
