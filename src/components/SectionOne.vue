<template>
  <div class="position-realive bg-image section-one-img">
    <div class="page-section" id="section-one">
      <div class="container">
        <div class="row">
          <div class="col-lg-5 py-3">
            <div class="img-place mobile-preview shadow wow zoomIn">
              <img src="https://surf.dev/wp-content/uploads/2021/02/twim_case_new.png" alt="" />
            </div>
          </div>
          <div class="col-lg-6 py-3 mt-lg-5">
            <div class="iconic-list">
              <div class="iconic-item wow fadeInUp">
                <div class="iconic-md iconic-text bg-warning fg-white rounded-circle">
                  <span class="mai-cube"></span>
                </div>
                <div class="iconic-content">
                  <h5>Do you trade for passive income?</h5>
                  <p class="fs-small">
                    Business is centered on trust, and our quickest payout will demonstrate this.
                    How about your trading, is it prepared for the change? Changes to the trading
                    platform and commissions that are superior. Let's alter your method of making a
                    profit.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="page-section" id="section-two">
      <div class="container">
        <div class="row">
          <div class="col-lg-6 offset-lg-1 py-3 mt-lg-5 wow fadeInUp">
            <h1 class="mb-4">Do you have any idea how you'll pay for your trade?</h1>
            <p class="mb-4">
              Crypto currency has revolutionized the way we pay for goods and services online.
              Crypto payment helps people break away from traditional banking practices and gives
              them more control over their wealth. Crypto Accounts are not linked to personal
              identity, offering greater privacy and anonymity when making payments. Crypto's has
              faster processing time for payments and highly Secure compared to other payment
              methods..
            </p>
            <a href="#" class="btn btn-outline-primary rounded-pill">How it works</a>
          </div>
          <div class="col-lg-5 py-3">
            <div class="img-place mobile-preview shadow wow zoomIn">
              <img
                src="https://www.forex.com/en-us/-/media/project/gain-capital/forex/feature-images/platforms/overview/platforms-overview-statichero-compress.png?h=550&iar=0&w=832"
                alt=""
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
h5 {
  font-size: 56px;
}

.section-one-img {
  background-image: url('../assets/img/pattern_1.svg');
}

.bg-image {
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}

.img-place {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
  width: 100%;
  height: 100%;
  text-align: center;
  overflow: hidden;
}

.img-place > img {
  width: 100%;
  height: 100%;
}

.img-place.w-auto > img {
  width: auto;
  max-width: 100%;
}

.img-place.h-auto > img {
  height: auto;
  max-height: 100%;
}

.img-place.custom-size > img {
  width: unset;
  height: unset;
}

.page-section {
  position: relative;
  padding-top: 100px;
  padding-bottom: 100px;
}

.page-section:not(.fg-white) h1,
.page-section:not(.fg-white) h2,
.page-section:not(.fg-white) h3 {
  color: #6b6872;
}

.mobile-preview {
  width: 100%;
  /* max-width: 233px; */
  height: auto;
  border-radius: 30px;
}
</style>
