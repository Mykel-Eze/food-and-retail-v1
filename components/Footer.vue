<template>
  <footer>
      <div class="row">
          <div class="container">
              <div class="footer-contents-wrapper">
                  <div class="footer-content-block footer-logo-block">
                      <router-link to="/" @click="scrollToTop()">
                          <img src="../assets/images/japtini-logo.png" alt="Japtini" class="footer-logo">
                      </router-link>
                      <div class="footer-social-wrapper">
                          <a href="http://facebook.com" target="_blank" rel="noopener noreferrer">
                            <img src="../assets/images/facebook.svg" alt="facebook" class="social-icons">
                          </a>
                          <!-- <a href="http://instagram.com" target="_blank" rel="noopener noreferrer">
                            <img src="../assets/images/instagram.svg" alt="instagram" class="social-icons">
                          </a> -->
                          <a href="https://twitter.com" target="_blank" rel="noopener noreferrer">
                            <img src="../assets/images/twitter.svg" alt="twitter" class="social-icons">
                          </a>
                          <a href="https://instagram.com" target="_blank" rel="noopener noreferrer">
                            <img src="../assets/images/instagram.svg" alt="instagram" class="social-icons">
                          </a> 
                          <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer">
                            <img src="../assets/images/linkedin.svg" alt="linkedin" class="social-icons">
                          </a>
                          <a href="https://youtube.com" target="_blank" rel="noopener noreferrer">
                            <img src="../assets/images/youtube.svg" alt="youtube" class="social-icons">
                          </a>
                      </div>
                  </div>
                  <div class="footer-content-block">
                      <h4 class="footer-sec-title">Headquarters</h4>
                      <div class="footer-sec-content">
                          Raymond Court, NA, Westlands District, P.O.Box 54549,  Nairobi Kenya
                      </div>
                  </div>
                  <div class="footer-content-block">
                      <h4 class="footer-sec-title">Order & inquires</h4>
                      <div class="footer-sec-content">
                          <div class="inq email-inq">
                              <span>Interested in special order?</span> <br />
                              <a href="mailto:info@japtinifoods.com" class="">
                                  <span>info@japtinifoods.com</span>
                              </a> <br />
                              <a href="tel:+254710595297" class="">
                                  <span>+254 710 595297</span>
                              </a>
                          </div>
                      </div>
                  </div>
                  <div class="footer-content-block">
                      <h4 class="footer-sec-title">Sign up for the newsletter</h4>
                      <div class="footer-sec-content">
                            <div class="subscribe-form-wrapper">
                                <form action="#" id="newsletter-form">
                                    <div class="flex-div input-field">
                                        <input id="subscriber-email" placeholder="Enter your e-mail…" type="email" required />
                                        <button class="btn subscribe-submit pry-bg">Get Started</button>
                                    </div>
                                </form>
                            </div>
                      </div>
                  </div>
              </div>
          </div>
          <div class="footer-credit-wrapper">
              <div class="row">
                  <div class="container">
                      <div class="copyright-div">
                          <p>
                            This website uses <a href="/" target="_blank" rel="noopener noreferrer" class="pry-color">Cookies <span class="pp-font">↗</span></a> 
                            We use cookies to personalise content and ads, to provide social media 
                            features and to analyse our traffic. The content on this website does not constitute a complete description of Japtini Food and Retail. By using this website, you accept our 
                            <a href="/" target="_blank" rel="noopener noreferrer" class="pry-color">Terms of Use</a> and 
                            <a href="/" target="_blank" rel="noopener noreferrer" class="pry-color">Privacy Policy</a>.
                          </p>
                      </div>
                      <div class="footer-sub-wrapper flex-div">
                          <div>© 2022 Japtini Food and Retails. All Rights Reserved.</div>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: "footer-section",
    methods:{
        scrollToTop() {
            window.scrollTo(0, 0);
        }
    }
}
</script>

<style scoped src="..\assets\css\footer.css"></style>
