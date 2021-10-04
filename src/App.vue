<template>
  <div id="app">
    <Header />
    <Services />
    <Company />
    <Projects />
    <Results />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Services from './components/services.vue'
import Company from './components/company.vue'
import Projects from './components/projects.vue'
import Results from './components/results.vue'
export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Services,
    Company,
    Projects,
    Results
  }
}
</script>

<style lang="scss">
@import './assets/Style/brandColors.scss';
@import './assets/Style/general.scss';
@import '~@fortawesome/fontawesome-free/css/all.min.css';
#App {
  max-width: 100vw;

}
.color-title {
    background-color: rgba( $blueLagoon, .15);
    color: $blueLagoon;
  }

</style>
