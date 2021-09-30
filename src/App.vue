<template>
  <div id="app">
    <Header />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/Style/brandColors.scss';
h1 {
  color: $santaFe;
}


</style>
