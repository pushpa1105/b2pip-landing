<script setup>
import { ref } from 'vue'

const formData = ref({
  name: '',
  email: '',
  phone: ''
})

const submitForm = () => {
  alert('Form Submitted')
}
</script>

<template>
  <button
    class="btn signup-btn btn-ring"
    type="button"
    data-bs-toggle="offcanvas"
    data-bs-target="#offcanvasBottom"
    aria-controls="offcanvasBottom"
  >
    <img src="../assets/img/signup.png" alt="" />
  </button>

  <div
    class="offcanvas offcanvas-bottom"
    tabindex="-1"
    id="offcanvasBottom"
    aria-labelledby="offcanvasBottomLabel"
    data-bs-scroll="true"
  >
    <div class="offcanvas-header w-75 m-auto justify-content-center">
      <h1>Join Us</h1>
      <button
        type="button"
        class="btn-close text-reset"
        data-bs-dismiss="offcanvas"
        aria-label="Close"
      ></button>
    </div>
    <div class="offcanvas-body small">
      <form class="signup-form d-flex flex-wrap justify-content-center">
        <div class="d-flex flex-column">
          <label for="username">Name</label>
          <input type="text" placeholder="Name" id="name" v-model="formData.name" />
        </div>

        <div class="d-flex flex-column">
          <label for="password">Email</label>
          <input type="email" placeholder="Email" id="email" v-model="formData.email" />
        </div>

        <div class="d-flex flex-column">
          <label for="Phone">Phone</label>
          <input type="text" placeholder="Phone" id="phone" v-model="formData.phone" />
        </div>

        <a
          href="#"
          class="btn btn-outline-primary rounded-pill sign-btn"
          @click="submitForm"
          data-bs-dismiss="offcanvas"
          >Sign Up</a
        >
      </form>
    </div>
  </div>
</template>

<style>
.sign-btn {
  text-align: center;
  align-items: center;
  display: flex;
  margin: auto 0 2px 10px;
  /* height: fit-content; */
  width: 150px;
  justify-content: center;
  height: 50px;
}

.button {
  min-width: 300px;
  min-height: 60px;
  /* font-family: 'Nunito', sans-serif; */
  font-size: 22px;
  text-transform: uppercase;
  letter-spacing: 1.3px;
  font-weight: 700;
  color: #313133;
  border: none;
  border-radius: 1000px;
  transition: all 0.3s ease-in-out 0s;
  cursor: pointer;
  outline: none;
  position: relative;
  padding: 10px;
}

.btn-ring::before {
  content: '';
  border-radius: 1000px;
  min-width: calc(300px + 12px);
  min-height: calc(60px + 12px);
  border: 6px solid #c9f73a;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  opacity: 0;
  transition: all 0.3s ease-in-out 0s;
}

.btn-ring::after {
  content: '';
  width: 30px;
  height: 30px;
  border-radius: 100%;
  border: 6px solid #c9f73a;
  position: absolute;
  z-index: -1;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  animation: ring 1.5s infinite;
}

.btn-ring:hover::after,
.btn-ring:focus::after {
  animation: none;
  display: none;
}

@keyframes ring {
  0% {
    width: 30px;
    height: 30px;
    opacity: 1;
  }

  100% {
    width: 300px;
    height: 300px;
    opacity: 0;
  }
}
</style>

<style lang="scss">
.signup-btn {
  position: fixed;
  bottom: 0;
  z-index: 999;
}

.signup-btn img {
  width: 10vw;
}

.signup-form {
  width: 75%;
  margin: auto;
}

.signup-form label {
  font-size: 16px;
  font-weight: 500;
}

.signup-form input {
  height: 50px;
  margin: 5px;
  padding: 5px;
  border-radius: 10px;
  border: 0;
  box-shadow:
    rgba(0, 0, 0, 0.09) 0px 2px 1px,
    rgba(0, 0, 0, 0.09) 0px 4px 2px,
    rgba(0, 0, 0, 0.09) 0px 8px 4px,
    rgba(0, 0, 0, 0.09) 0px 16px 8px,
    rgba(0, 0, 0, 0.09) 0px 32px 16px;
}

.signup-form input:focus-visible {
  border: 0 !important;
  border-inline: none !important;
  outline: none;
}

btn-check:focus + .btn,
.btn:focus {
  outline: 0;
  box-shadow: none !important;
}

.offcanvas.show {
  background: rgba(255, 255, 255, 0.5);
  backdrop-filter: blur(4px);
}

.btn-outline-primary {
  color: #c9f73a;
  border-color: #c9f73a;
}

.btn-outline-primary:hover {
  color: #000;
  background-color: #c9f73a;
  border-color: #c9f73a;
}

.offcanvas-header .btn-close {
  position: absolute;
  right: 30px;
}

.offcanvas-bottom {
  height: 25vh;
}

@media screen and (max-width: 880px) {
  .offcanvas-bottom {
    height: 50vh;
  }
  .signup-form div {
    width: 100%;
    margin: auto;
  }
}
</style>
