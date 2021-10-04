<template>
  <div class="wrapper">      
      <div class="row-top">
            <h3>we do more for everyone</h3>
            <h1>actions & <span>projects</span></h1>
            <div class="mini-nav">
                <div v-for="(item, index) in navList" :key="index" class="nav-item">
                    {{item}}
                </div>

            </div>
      </div>
      <div class="row-bot">
          <div v-for="(item, index) in card" :key="index" class="card">
              <img :src="require(`../${item.img}`)" alt="">
              <h1>{{item.text}}</h1>
          </div>
      </div>
  </div>
</template>

<script>
import * as List from '@/assets/Lists/lists.js'
export default {
    name: 'Projects',
    data() {
        return {
            navList: List.projectNav,
            card: List.projectCard,
        }
    }

}
</script>

<style lang="scss" scoped>
@import '../assets/Style/brandColors.scss';

.wrapper {
    width: 100vw;
    background-color: $white;
    .row-top {
        padding: 10vh 0 10px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        h3 {
            color: lighten($blueLagoon, 10%);
            padding-bottom: 30px;
            text-transform: uppercase;
        }
        h1 {
            font-size: 3.5rem;
            text-transform: capitalize;
            font-weight: 900;
            span {
                color: $blueLagoon;
                background-color: rgba( $blueLagoon, .2);
                padding: 0 10px;
            }
        }
        .mini-nav {
            padding: 20px;
            display: flex;
            div {
                padding:10px 20px;
                font-size: 1.6rem;
                color: darken($pumice, 20%);
            }
            .nav-item:first-child {
                background-color: rgba($blueLagoon, .2);
                padding: 10px;
                color: darken($pumice, 30%);
            }      
        }
    }
    .row-bot {
        width: 70vw;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        .card {
            width: calc((100% / 3) - 30px );
            position: relative;
            padding: 15px;
            img {
                width: 100%;
                filter: brightness(50%);
                border-radius: 1rem;

            }
            h1 {
                position: absolute;
                bottom: 70px;
                left: 0;
                color: $white;
                text-align: center;
            }

        }
    }

}
</style>