<template>
  <div id="app-wrapper">
    <Navbar />
    <div id="main-contents-wrapper">
      <Nuxt />
    </div>
    <Footer />
  </div>
</template>

<script>
// import $ from 'jquery'

import Navbar from '~/components/Navbar'
import Footer from '~/components/Footer'
export default {
  name: 'DefaultLayout',
  components: { Navbar, Footer },
  mounted () {
    const $ = require('jquery')

    $(window).scroll(function () {
      $('nav.main-nav').toggleClass('scrolled-nav', $(this).scrollTop() > 50)
    })
  }
}
</script>

<style>
div#nav {
  float: left;
  width: 100%;
  overflow-x: hidden;
  position: relative;
  min-height: 100vh;
}

div#main-contents-wrapper {
  padding-top: 100px;
}
</style>
