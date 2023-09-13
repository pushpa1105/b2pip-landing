<script setup>
import AdditionalSection from './components/AdditionalSection.vue'
import Footer from './components/Footer.vue'
import SignUp from './components/SignUp.vue'
import Leverage from './components/Leverage.vue'
import CopyTrading from './components/CopyTrading.vue'
import InnovativeSection from './components/InnovativeSection.vue'
import MainPage from './components/MainPage.vue'
</script>

<template>
  <SignUp />

  <MainPage />

  <CopyTrading />
  <Leverage />
  <AdditionalSection />
  <InnovativeSection />




  <Footer />
</template>

<style lang="scss">
/*** FONTS ***/

/*** VARIABLES ***/
/* Colors */
$black: #1d1f20;
$blue: #83e4e2;
$green: #a2ed56;
$yellow: #fddc32;
$white: #fafafa;

/*** EXTEND ***/
/* box-shadow */
%boxshadow {
  box-shadow:
    0.25rem 0.25rem 0.6rem rgba(0, 0, 0, 0.05),
    0 0.5rem 1.125rem rgba(75, 0, 0, 0.05);
}

/*** STYLE ***/
*,
*:before,
*:after {
  box-sizing: border-box;
}

html,
body {
  margin: 0;
  padding: 0;
}

body {
  background-color: $white;
  color: $black;
}

main {
  display: block;
  margin: 0 auto;
  max-width: 40rem;
  padding: 1rem;
}

.first {
  display: flex;
  flex-wrap: wrap;
  width: 65%;
  margin: auto;
  margin-top: 7em;
}

.trade-img {
  margin: auto;
  margin-top: -5vh;
  width: 17vw;
}

ol.gradient-list {
  counter-reset: gradient-counter;
  list-style: none;
  padding-left: 1rem;
  display: inline-grid;

  > li {
    background: white;
    border-radius: 0 0.5rem 0.5rem 0.5rem;
    @extend %boxshadow;
    counter-increment: gradient-counter;
    margin-top: 1rem;
    min-height: 3rem;
    padding: 1rem 1rem 1rem 3rem;
    position: relative;
    display: inline-block;
    max-width: 80vw;
    box-shadow: 10px 15px 25px 0 rgba(0, 0, 0, 0.2);
    transition: all 0.5s cubic-bezier(0.645, 0.045, 0.355, 1);
    cursor: pointer;
    margin: 0 0 1em 1em;

    &::before,
    &::after {
      background: linear-gradient(135deg, $blue 0%, $green 100%);
      border-radius: 1rem 1rem 0 1rem;
      content: '';
      height: 3rem;
      left: -1rem;
      overflow: hidden;
      position: absolute;
      top: -1rem;
      width: 3rem;
    }

    &::before {
      align-items: flex-end;
      @extend %boxshadow;
      content: counter(gradient-counter);
      color: $black;
      display: flex;
      font: 900 1.5em/1 'Montserrat';
      justify-content: flex-end;
      padding: 0.125em 0.25em;
      z-index: 1;
    }

    &:hover {
      box-shadow: 0 0 10px #c9f73a;
    }

    @for $i from 1 through 5 {
      &:nth-child(10n + #{$i}):before {
        background: linear-gradient(
          135deg,
          rgba($green, $i * 0.2) 0%,
          rgba($yellow, $i * 0.2) 100%
        );
      }
    }

    @for $i from 6 through 10 {
      &:nth-child(10n + #{$i}):before {
        background: linear-gradient(
          135deg,
          rgba($green, 1 - (($i - 5) * 0.2)) 0%,
          rgba($yellow, 1 - (($i - 5) * 0.2)) 100%
        );
      }
    }

    + li {
      margin-top: 2rem;
    }
  }
}

li::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background: #ffee10;
  transition: 0.5s;
  transform: scale(0.9);
  z-index: -1;
}

li:hover::before {
  transform: scale(1.1);
  box-shadow: 0 0 15px #ffee10;
}

li:hover {
  // color: #ffee10;
  // box-shadow: 0 0 15px #ffee10;
  box-shadow: 0 0 15px #ffee10;
  // text-shadow: 0 0 5px #ffee10;
}

.main-page {
  background-image: url('./assets/img/bg_hero_1.svg');
  height: 100vh;
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}

h1 {
  margin: 0;
}

/* Header section */
.main-header {
  display: flex;
  justify-content: space-between;
  max-width: 1200px;
  margin: auto;
  max-height: 20vh;
}

.announcement {
  display: flex;
}

.announcement h2 {
  font-size: 5vw;
  margin: 0;
  position: relative;
  /* top: 1vh; */
  right: -4.5%;
  color: #f75e0a;
  height: fit-content;
}

.announcement-img {
  width: 8em;
  object-fit: contain;
}

.announcement-list {
  padding: 10px;
  border: 1px solid #f75e0a;
  height: max-content;
  margin: auto;
  border-radius: 30px;
  box-shadow: 0 0 10px #f75e0a;
  background: black;
  color: #c9f73a !important;
}

.logo {
  margin: auto 0.5em;
}

.logo img {
  width: 10em;
  max-width: 100%;
  height: auto;
}

@media screen and (max-width: 768px) {
  .topics {
    width: 95%;
    margin: 0;
  }

  .first {
    width: 85%;
    margin: auto;
    margin-top: 10%;
  }

  .trade-img {
    display: none;
  }

  ol.gradient-list > li {
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
    margin: 0;
  }
  .announcement h2 {
    font-size: 56px;
    top: 1.5vh;
    right: -8%;
  }
}
@media screen and (min-width: 2000px) {
  .first {
    width: 40%;
  }
}

@media screen and (max-width: 1111px) {
  .trade-img {
    display: none;
  }
}

@media screen and (max-width: 400px) {
  .signup-btn img {
    width: 55px;
  }
}

@media screen and (min-width: 1100px) and (max-width: 1400px) {
  .first {
    width: 70%;
    margin-left: 0;
    margin-right: 0;
  }
}
</style>
