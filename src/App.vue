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
@import './assets/Style/general.scss';
@import '~@fortawesome/fontawesome-free/css/all.min.css';
#App {
  height: 100vh;
  width: 100vw;
}


</style>
