<template>
  <div class="wrapper">
      <div class="top">
        <div class="info">
          <img :src="require(`../assets/img/svg-7.svg`)" alt="logo Nex Gen">
          <p>
            A Functional HTML template
            for Coporate & Business
          </p>
          <span>
            <i class="fas fa-phone-alt"></i>
            +1 (305) 1234-5678
          </span>
          <span>
              <i class="fas fa-envelope"></i>
              hello@example.com
          </span>
          <span>
              <i class="fas fa-map-marker-alt"></i>
              MAIN AVENUE, 987
          </span>
          <div class="btn">
                  GET IN TOUCH
          </div>
        </div>
        <div class="container">
          <h2>
            About
          </h2>
          <p v-for="(item, index) in first" :key="index">
              <i class="fas fa-chevron-right"></i>
              {{item}}
          </p>
        </div>
        <div class="container">
          <h2>
            Services
          </h2>
          <p v-for="(item, index) in second" :key="index">
              <i class="fas fa-chevron-right"></i>
              {{item}}
          </p>
        </div>
        <div class="container">
          <h2>
            Support
          </h2>
          <p v-for="(item, index) in third" :key="index">
              <i class="fas fa-chevron-right"></i>
              {{item}}
          </p>
        </div>
      </div>
      <div class="bottom">
        <span>
          Enjoy the low price. We are tracking any intention of piracy.
        </span>
        <span>
          <i class="far fa-copyright"></i>
          2020 NEXGEN is Proudly Powered by <span id="color">Codings</span>.
        </span>
      </div>
      <a href="#">
        <i class="fas fa-arrow-circle-up"></i>
      </a>
  </div>
</template>

<script>
import * as Link from '@/assets/Lists/lists.js'
export default {
    name: 'Footer',
    data() {
      return{
        first: Link.about,
        second: Link.services,
        third: Link.support
      }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/Style/brandColors.scss';
.wrapper {
  background-color:$woodsmoke;
  height: 70vh;
  padding-top: 12vh;
  color: lighten($shark, 60%);
  position: relative;

  .top {
    margin:0 auto;
    display: flex;
    width:60%;
    height:420px;
    .info {
      width:calc((100% / 4) - 60px);
      margin: 10px 40px 10px 10px;
      height: 400px;
      display: flex;
      flex-direction: column;
      p, span {
        padding: 15px 0;
        font-size: 1.1rem;
      }
      img {
        width: 180px;
        
      }
      .btn {
        border: 1px solid $blueLagoon;
        border-radius: .3rem;
        width: 160px;
        height: 50px;
        padding: 15px 20px;
        color: $white;
      }
    }
    .container {
      width:calc((100% / 4) - 20px);
      margin:10px;
      padding: 30px 40px;
      height: 330px;
      border-radius: .3rem;
      display: flex;
      flex-direction: column;
      background-color: #19191F;
      h2 {
        padding-bottom: 20px;
        color: lighten($white, 10%);
      }
      p {
        i {
          padding-right: 5px;
        }
        font-size: 1.1rem;
        padding: 5px 0;
      }
    }
  }
  .bottom {
    position: absolute;
    width: 100%;
    height:100px;
    display: flex;
    justify-content:space-evenly;
    background-color: darken($woodsmoke, 5%);
    align-items: center;
    bottom:0;
    left:0;
    // transform:translate(-50%, -50%)
  }
  .fa-arrow-circle-up {
    position: absolute;
    right: 30px;
    bottom:30px;
    font-size: 3.5rem;
    color: #1A1A1D;
  }
}
</style>