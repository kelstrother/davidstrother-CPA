<template>
  <div class="layout">
    <div class="sidebar">
    </div>
    <div class="logo-container">
      <g-image class="brand" src="../Branding Logo.png" width="400"/>
    </div>
    <div class="hero-section">
      <img src="../building-hero.png" alt="" class="hero-img">
    </div>
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>
<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat+Alternates:wght@100;200;300;400;500;600;700;800;900&display=swap');
* {
  margin:0;
  padding:0;
  box-sizing: border-box;
}
body {
  /* background-color: rgba(0, 0, 0, 0); */
  font-family: "Montserrat Alternates";
  overflow: hidden;
}
.layout {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-template-rows: repeat(5, 1fr);
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  background-color: rgb(221, 197, 132);
  width: 100vw;
  height: 100vh;
}
.logo-container {
  margin: 0 15rem 2rem 0;
  grid-column: 2;
  grid-row: 5;
  z-index: 10;
}
.brand {
  width: 400px;
}
.hero-section {
  grid-column: 1/6;
  grid-row: 1/6;
  /* background-image: "../artem-page-T7OP6oIbopQ-unsplash.jpg"; */
}
.hero-img {
  z-index: 0;
  width: 100%;
  height: 100%;
}
</style>
