<template>
  <Layout>
    <!-- <div class="container"> -->
      <!-- <g-image class="dark-filter" src="../light-filter_hero.jpg"/> -->
      <!-- <div class="logo-container">
        <g-image class="brand" src="../ds-cpa_logo.svg" width="350"/>
      </div> -->
        <!-- <g-image class="vector-logo" src="../mobile-vector-logo.svg" width="300"/> -->
    <!-- </div> -->
  </Layout>
</template>

<script>
import Layout from '~/layouts/Default.vue'
export default {
  components: {
    Layout
  }
}
</script>

<style>
  body {
    font-family: "Montserrat Alternates";
  }

  .brand {
    z-index: 15;
    grid-column: 1;
    grid-row: 1/5;
  }
  .vector-logo {
    position: fixed;
    top: 23%;
    left: 5%;
  }
  #mobile-vector-logo {
    stroke-dasharray: 1;
   animation: fill-line 3s ease both;
  }
  .svg-path {
   stroke-dasharray: 1;
   animation: fill-line 3s ease both;
}
@keyframes fill-line {
   from {
      stroke-dashoffset: 1;
   }
    to {
       stroke-dashoffset: 0;
    }
}
</style>
