<template>
  <div>
    <nav class="main-nav">
        <div class="container">
            <div class="nav-wrapper">
                <router-link to="/" class="brand-logo" @click="scrollToTop()">
                    <img src="../assets/images/japtini-logo.png" alt="Japtini" class="logo">
                </router-link>

                <ul class="dn-mobile ul-nav" id="nav-mobile-2">
                    <li>
                        <a href="#" data-target="slide-out" class="sidenav-trigger sec-color right">
                            <img src="../assets/images/menu.svg" alt="menu" />
                        </a>
                    </li>
                </ul>

                <ul id="nav-mobile" class="right hide-on-med-and-down">
                    <li>
                        <router-link to="/" class="" @click="scrollToTop()">
                            <span>Home</span>
                        </router-link>
                    </li>
                    <li>
                        <router-link to="/about" class="" @click="scrollToTop()">
                            <span>About</span>
                        </router-link>
                    </li>
                    <!-- <li>
                        <a href="#partner-form-modal" class="modal-trigger">
                            <span>Become a Partner</span>
                        </a>
                    </li> -->
                    <li>
                        <router-link to="/faq" class="" @click="scrollToTop()">
                            <span>FAQ</span>
                        </router-link>
                    </li>
                    <li class="contact-us-li">
                        <a href="#partner-form-modal" class="modal-trigger" @click="scrollToTop()">
                            <button class="nav-pry-btn btn pointer flex-div">
                                <span>Become a Partner</span> <span class="btn-icon">&#8250;</span>
                            </button>
                        </a>
                    </li>
                </ul>
              </div>
        </div>
    </nav>

    <ul id="slide-out" class="sidenav">
        <div class="sidenav-logo">
            <router-link to="/" class="sidenav-close" @click="scrollToTop()">
                <img src="../assets/images/japtini-logo.png" alt="Japtini" class="logo">
            </router-link>
        </div>
        <li>
            <router-link to="/" class="sidenav-close" @click="scrollToTop()">
                <span>Home</span>
            </router-link>
        </li>
        <li>
            <router-link to="/about" class="sidenav-close" @click="scrollToTop()">
                <span>About</span>
            </router-link>
        </li>
        <li>
            <router-link to="/faq" class="sidenav-close" @click="scrollToTop()">
                <span>FAQ</span>
            </router-link>
        </li>
        <li>
            <a href="#partner-form-modal" class="sidenav-close modal-trigger">
                <span>Become a Partner</span>
            </a>
        </li>
        <li class="contact-us-li">
            <a href="#partner-form-modal" class="modal-trigger">
                <button class="nav-pry-btn btn pointer">
                    Become a Partner<span>&#62;</span>
                </button>
            </a>
        </li>
    </ul>

    <PartnerFormModal />
  </div>
</template>

<script>
import PartnerFormModal from './PartnerFormModal.vue';

export default {
  name: "Navbar",
  components: { PartnerFormModal },
  mounted() {
    const M = require('materialize-css')

    document.addEventListener("DOMContentLoaded", function() {
      var elemsSidenav = document.querySelectorAll(".sidenav");
      M.Sidenav.init(elemsSidenav)

      var elemsModal = document.querySelectorAll('.modal');
      M.Modal.init(elemsModal);
    });
  },
  methods:{
    scrollToTop() {
        window.scrollTo(0, 0);
    }
  }
};
</script>

<style scoped src="..\assets\css\navbar.css"></style>
