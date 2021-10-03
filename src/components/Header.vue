<template>
  <div id="header">
    <Nav />
    <Jumbo />
  </div>
</template>

<script>
import Nav from './Nav.vue'
import Jumbo from './Jumbo.vue'
export default {
  name: 'Header',
  components: {
    Nav,
    Jumbo,
  }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#header {
    background-repeat: no-repeat;
    background-position: 50% 40%;
    background-image: url("../assets/img/bg-parallax.png");
    height:80vh;
    width: 100vw;
}

</style>
