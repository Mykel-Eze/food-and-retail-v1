<template>
  <div id="main-wrapper">
    <section id="about-home">
      <div class="row full-height">
        <div class="container full-height">
          <div class="home-title-wrapper">
            <div class="home-title-block">
              <h1 class="page-title">About</h1>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="about-txt-1" class="text-section section">
      <div class="row">
        <div class="container">
          <p>
            We are your partner in providing premium quality authentic fine food products to your discerning customers,
            simplifying trade across borders by providing personalized and innovative end-to-end solutions in an ever-changing
            agricultural world. Japtini Food and Retail will bridge the gap by providing quality dry foods (including but
            not limited to rice and wheat at competitive prices for Africans focusing on the top 20 consuming countries of
            wheat across the continent, from an understanding of the bridges in service, communication and quality experienced
            by many brands in the African market.
          </p>
        </div>
      </div>
    </section>

    <section id="block-quote-section" class="section">
      <div class="row full-height">
        <div class="container full-height">
          <div class="block-quote-div">
            <span class="rel">
              With premium quality grains made available on demand, we offer 100% sustainably grown products from Africa, among
              other prime global locations — no shortcuts, best quality, no cutting corners!
            </span>
          </div>
        </div>
      </div>
    </section>

    <section id="about-txt-2" class="text-section section">
      <div class="row">
        <div class="container">
          <p>
            We actively promote sustainable farming, with a focus on preserving nature, and maintaining the health and viability
            of agricultural communities. With corporate policies and partner guidelines that espouse sustainability and
            authenticity, every food product with Japtini comes with the guarantee that you are getting premium quality fine foods.
          </p>
        </div>
      </div>
    </section>

    <section id="our-process" class="section">
      <div class="row">
        <div class="container">
          <h4 class="section-title center">Our Process</h4>

          <div class="process-block-wrapper">
            <div class="process-block">
              <img src="../assets/images/process-1.svg" alt="process icon" class="process-icon">
              <p class="process-block-desc">
                Through Alluvial, Smallholder farmers are provided with storage facilities and their produce is
                warehoused for off takers Immediately after harvest.
              </p>
            </div>
            <div class="process-block">
              <img src="../assets/images/process-2.svg" alt="process icon" class="process-icon">
              <p class="process-block-desc">
                Smallholder farmers are provided with market linkage services; their produce is taken by Japtini
                and sold to offtakers that had secured agreements earlier.
              </p>
            </div>
            <div class="process-block">
              <img src="../assets/images/process-3.svg" alt="process icon" class="process-icon">
              <p class="process-block-desc">
                Smallholders pay a percentage of their produce to Japtini food and retail for the processing services
                received, and the proceeds from the remaining produce is given to the farmers.
              </p>
            </div>
            <div class="process-block">
              <img src="../assets/images/process-4.svg" alt="process icon" class="process-icon">
              <p class="process-block-desc">
                Alluvial provides smallholder farmers with opportunities to process their farm produce by providing all
                processing and marketing solutions.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>


<script>
// import M from "materialize-css";
export default {
  name: 'About',
  mounted() {
    const M = require('materialize-css')

    document.addEventListener("DOMContentLoaded", function() {
      var elemsTab = document.querySelectorAll('.tabs');
      M.Tabs.init(elemsTab);
    });
  }
}
</script>

<style src="../assets/css/about.css" scoped></style>
