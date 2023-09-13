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
      <div class="logo">
        <img src="../assets/img/logo.svg" alt="logo" />
      </div>
      <div class="announcement">
        <div class="announcement-list text-white">Get your customer today with us!!!</div>
        <h2>5</h2>
        <img src="../assets/img/announcement_art.png" alt="announcement-img" class="announcement-img" />
      </div>
    </div>

    <!-- main topics -->
    <div class="first">
      <div class="topics">
        <ol class="gradient-list">
          <li @click="scrollToSection('copy-trading')">Copy Trading - Trading becomes investment.</li>
          <li @click="scrollToSection('leverage')">
            No mark-up spread Trade with Trust Upto 1:500 leverage
          </li>
          <li @click="scrollToSection('trading-account')">What is your choice of trading account?</li>
          <li @click="scrollToSection('section-one')">Do you trade for passive income?</li>
          <li @click="scrollToSection('section-two')">
            Do you have any idea how you'll pay for your trade?
          </li>
          <!-- <li @click="scrollToSection('section-five')">
            Is your trading platform as innovative as your trading ideas?
          </li> -->
        </ol>
      </div>
      <div class="trade-img">
        <img src="https://platinumfx.io/assets/images/mob.png" alt="" />
      </div>
    </div>

    <!-- main topics -->
  </div>
</template>
