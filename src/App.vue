<template>
  <div id="app">
    <Header />
    <Services />
    <Company />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Services from './components/services.vue'
import Company from './components/company.vue'
export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Services,
    Company
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
.color-title {
    background-color: rgba( $blueLagoon, .15);
    color: $blueLagoon;
  }

</style>
