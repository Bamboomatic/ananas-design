<template>
  <img class="logo" alt="Ananas logo" src="../public/assets/logo.png">
  <Header/>
  <Gallery/>
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
}
@font-face {
  font-family: "Praho";
  src: local("Praho"),
   url(../public/Praho-Black.ttf) format("truetype");
}
.logo{
  height: 15vh;
}
</style>
