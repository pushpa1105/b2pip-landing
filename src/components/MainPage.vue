<script setup>
const scrollToSection = (sectionId) => {
  const targetSection = document.getElementById(sectionId)
  if (targetSection) {
    targetSection.scrollIntoView({ behavior: 'smooth' })
  }
}
</script>
<template>
  <div class="main-page">
    <div class="main-header">
      <div class="announcement">
        <img src="../assets/img/announcement.png" alt="announcement-img" class="announcement-img" />
        <h2>5</h2>
        <div class="announcement-list text-white">Get your customer today with us!!!</div>
      </div>
      <div class="logo">
        <img src="../assets/img/logo.svg" alt="logo" />
      </div>
    </div>

    <!-- main topics -->
    <div class="first">
      <div class="topics">
        <ol class="gradient-list">
          <li @click="scrollToSection('section-one')">Do you trade for passive income?</li>
          <li @click="scrollToSection('section-two')">
            Do you have any idea how you'll pay for your trade?
          </li>
          <li @click="scrollToSection('section-three')">What is your choice of trading account?</li>
          <li @click="scrollToSection('section-four')">
            No mark-up spread Trade with Trust Upto 1:500 leverage
          </li>
          <li @click="scrollToSection('section-five')">
            Is your trading platform as innovative as your trading ideas?
          </li>
        </ol>
      </div>
      <div class="trade-img">
        <img src="https://platinumfx.io/assets/images/mob.png" alt="" />
      </div>
    </div>

    <!-- main topics -->
  </div>
</template>
