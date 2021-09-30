<template>
  <div>
    <h1> HEADER</h1>
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
    Jumbo
  }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
