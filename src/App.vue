<template>
  <div id="app">
    <Header />
    <Services />
    <Company />
    <Projects />
    <Results />
    <Form />
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
import Form from './components/form.vue'
export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Services,
    Company,
    Projects,
    Results,
    Form
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
.btn:hover,
.btn-left:hover,
.btn-right:hover {
  background-color: lighten($blueLagoon, 10%) !important;
  span {
    color: $white;
  }
}

</style>
