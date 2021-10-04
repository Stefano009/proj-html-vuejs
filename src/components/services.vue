<template>
  <div class="wrapper">
      <div class="inner">
          <h3>
              our business areas
          </h3>
          <h1>
              Exellence in <span class="color-title">Services</span>
          </h1>
          <div class="service-wrapper">
              <p>
             We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire. 
            </p>
          <div class="btn"> 
              see all
          </div>
          </div>
      </div>
      <div class="cards-wrapper">
          <div v-for="(item, index) in cards" :key="index" class="card">
              <div class="first-row">
                  <img :src="require(`../${item.img}`)" :alt="item.img">
                  <i class="fas fa-arrow-right"></i>
              </div>
              <h1>
                  {{item.title}}
              </h1>
              <p>
                  Lorem ipsum dolor sit amet,<br> consectetur adipiscing elit. 
              </p>
          </div>
      </div>
  </div>
</template>

<script>
import * as servicesCard from '@/assets/Lists/lists.js'
export default {
    name:'Services',
    data() {
        return {
            cards: servicesCard.servicesCard,
        }
    }

}
</script>

<style lang="scss" scoped>
@import '../assets/Style/brandColors.scss';
    .wrapper {
        height: 100vh;
        max-width: 100vw;
        background-color: #EEF4ED;
        .inner {
            width: 60%;
            margin: 0 auto;
            padding-top: 15vh ;
            h3 {
                color: lighten($blueLagoon, 8%);
                padding-bottom: 2vh;
                text-transform: uppercase;
                font-size: 0.9rem;
            }
            h1 {
                font-size: 3rem;
                padding-bottom: 20px;
                font-weight: 900;
                span {
                    padding: 0 10px;
                }
            }
            .service-wrapper {
                display: flex;
                justify-content: space-between;
                height:40px;
            }
            & p {
                padding: 10px;
                width: 70%;
                font-size: 1rem;
                color: gray;
            }
            & .btn {               
                text-transform: uppercase;
                text-align: center;
                padding-top: 10px;
                background-color: $blueLagoon;
                color: white;
                width: 10%;
                border-radius: .3rem;
           }
        }
        .cards-wrapper {
                width: 60%;
                margin: 30px auto;
                display: flex;
                flex-wrap: wrap;
                justify-content:center;
                align-items: center;
               .card {
                   width: calc((100% / 3) - 30px);
                   height: 250px;
                   margin:15px;
                   background-color: $white;
                   border-radius: .5rem;
                   padding-left: 30px;
                   .first-row {
                       display: flex;
                       justify-content: space-between;
                       height:calc((100% / 3) + 15px);
                       padding: 30px 20px;
                       img {
                           height: 50px;
                       }
                       i {
                           font-size: 1.5rem;
                           color: rgba($blueLagoon, 0.4);
                           padding-right: 20px;
                       }
                   }
                   h1 {
                       font-size: 1.5rem;
                       padding:0 0 30px 30px;
                   }
                   p {
                       padding-left: 30px;
                       font-size: 1.1rem;
                       color:gray;
                   }
               }
           }
    }
</style>