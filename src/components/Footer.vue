<template>
  <div class="page-footer-section bg-dark fg-white">
    <div class="container mb-5">
      <div class="row justify-content-center text-center wow fadeInUp">
        <div class="col-lg-8">
          <div class="text-center mb-3">
            <img src="../assets/favicon-light.png" alt="" height="80" />
          </div>
          <h3 class="mb-3 text-white">B2pip</h3>
          <p class="caption">
            We are a dynamic and innovative forex broker that empowers traders to take control of
            their financial future. Our mission is to provide users with the tools and resources
            they need to make the most informed trading decisions possible. At B2pip, we understand
            that traders are looking for opportunities to make their money work for them. That is
            why we offer a variety of trading instruments such as major currency pairs, spot energy,
            and metals. Our clients also have access to Ctrader, a well-known trading and charting
            platform.
          </p>

          <ul class="nav justify-content-center py-3">
            <li class="nav-item">
              <a
                href="https://b2pip.com/about-company"
                class="nav-link fg-white px-4"
                target="_blank"
                >About Company</a
              >
            </li>
            <li class="nav-item">
              <a href="https://b2pip.com/faq" class="nav-link fg-white px-4" target="_blank">FAQ</a>
            </li>
            <li class="nav-item">
              <a href="https://b2pip.com/kyc-policy" class="nav-link fg-white px-4" target="_blank"
                >KYC/AML Policy</a
              >
            </li>
            <li class="nav-item">
              <a
                href="https://b2pip.com/privacy-policy"
                class="nav-link fg-white px-4"
                target="_blank"
                >Privacy Policy</a
              >
            </li>
            <li class="nav-item">
              <a
                href="https://b2pip.com/get-in-touch"
                class="nav-link fg-white px-4"
                target="_blank"
                >Contact</a
              >
            </li>
            <li class="nav-item">
              <a
                href="https://b2pip.com/risk-disclosure"
                class="nav-link fg-white px-4"
                target="_blank"
                >Risk Disclosure</a
              >
            </li>
          </ul>
        </div>
      </div>
    </div>

    <!-- Please don't remove or modify the credits below -->
    <p class="text-center mt-4 wow fadeIn">
      Copyright &copy;
      <a href="https://b2pip.com/" class="fg-white fw-medium" target="_blank">b2pip.com</a>. All
      right reserved
    </p>
  </div>
</template>

<style>
.nav-item::before {
  content: none;
}
.nav-item:hover {
  box-shadow: none;
}
.page-footer-section {
  position: relative;
  padding-top: 10px;
  padding-bottom: 20px;
  background-color: #f0eef5;
}

.page-footer-section.bg-dark .caption {
  color: rgba(255, 255, 255, 0.6);
}

.page-footer-section.bg-dark hr {
  border-color: #4d4853;
}
.page-footer-section a,
.page-footer-section p {
  color: #b2b4bf;
}

.page-footer-section a:hover {
  color: #c9f73a;
  text-decoration: none;
}

.menu-link {
  position: relative;
  padding-left: 0;
  list-style: none;
}

.menu-link li {
  display: block;
  margin: 10px 0;
}

.menu-link li a {
  padding-top: 6px;
  padding-bottom: 6px;
  color: #b2b4bf;
}

.menu-link li a:hover {
  color: #c9f73a;
  text-decoration: none;
}

@media screen and (max-width: 768px) {
  .nav-item {
    min-width: 150px;
  }
}
</style>
