<template>
  <div class="white-wrapper">
    <img class="logo" alt="Ananas logo" src="../public/assets/logo.png">
  </div>
  <Header/>
  <div class="space"></div>
  <div class="white-wrapper">
    <Gallery/>
  </div>
  <Footer/>
</template>

<script>
import Header from './components/Header.vue'
import Gallery from './components/Gallery.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Gallery,
    Footer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  min-width: 360px;
}
body{
  margin: 0;
  background-image: url(../public/assets/background.jpg);
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;

}
@font-face {
  font-family: "Praho";
  src: local("Praho"),
   url(../public/Praho-Black.ttf) format("truetype");
}
.white-wrapper{
  width: 100%;
  background: white;
}
.logo{
  height: 15vh;
  background: white
}
.space{
  height: 40vh;
}
</style>
