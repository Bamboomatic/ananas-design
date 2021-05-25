<template>
  <div class="footer">
    
    <div class="contact">
      <div>sylvis1986@o2.pl</div>
      <div>+48 603 491 923</div>
      <div>Silesia</div>

    </div>
    <div class="copyright">	&copy; Ananas 2021</div>
 
  
  </div>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
  padding: 10px;
  margin: 0 auto;
  background: black;
  color:aliceblue;
  display: flex;
  justify-content: space-between;
}
.contact{
  display: flex;
  flex-direction: column;
  text-align: left;
  font-size: 0.8rem;
}
.copyright{
  margin-top: auto;
}
</style>
