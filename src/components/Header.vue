<template>
  <div class="header">
    <h1>{{ msg }}</h1>
  
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  padding: 10px;
  margin: 0 auto;
  background: black;
  color:aliceblue;
}
</style>
