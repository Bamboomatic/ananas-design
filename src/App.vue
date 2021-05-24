<template>
  <img class="logo" alt="Ananas logo" src="./assets/logo.png">
  <Header msg="Ananas Design"/>
  <Gallery/>
</template>

<script>
import Header from './components/Header.vue'
import Gallery from './components/Gallery.vue'

export default {
  name: 'App',
  components: {
    Header,
    Gallery
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
body{
  margin: 0;
}
.logo{
  height: 15vh;
}
</style>
