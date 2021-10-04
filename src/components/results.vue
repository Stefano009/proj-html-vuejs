<template>
    <div class="wrapper">
        <div class="big-row">
            <div class="column-row">
                <h3> WHAT ARE WE DOING</h3>
                <h1><span>Results</span> in Numbers</h1>
            </div>
            <div class="inner-row">
                <div v-for="(item, index) in numbers" :key="index" class="card">
                    <h1>{{item.number}}</h1>
                    <h2>{{item.text}}</h2>
                </div>
            </div>
        </div>
        <div class="small-row">
            <div v-for="(img, index) in imgs" :key="index" class="img">
            <img :src="require(`../${img.img}`)" alt="">
            </div>
        </div>
    </div>
</template>

<script>
import * as Link from '@/assets/Lists/lists.js'
export default {
    name: 'results',
    data() {
        return {
            numbers: Link.innerRow,
            imgs: Link.resultsPng
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/Style/brandColors.scss';
.wrapper {
    height: 90vh;
    .big-row {
        background-image: url("../assets/img/bg-7.jpg");
        height:70%;
        width: 100%;
        background-repeat: no-repeat;
        background-size: cover;
        background-position-y: center;
        .column-row {
            display: flex;
            flex-direction: column;
            justify-content:center;
            align-items: center;
            padding: 150px 0 0;
            h3 {
                color: lighten($blueLagoon, 10%);
            } 
            h1 {
                padding: 20px;
                font-size: 4rem;
                color: $white;
                font-weight: 900;
                span {
                    background-color: rgba($blueLagoon, .2);
                    padding:0 10px;
                }
            }
        }
        .inner-row {
            display: flex;
            color:$white;
            height: 50%;
            justify-content:center;
            .card {
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                padding: 70px;
                font-size: 1.5rem;
                h1 {
                    color: lighten($blueLagoon, 10%);
                }
                h2 {
                    font-size: 2rem;
                }
            }
        }
    }
    .small-row {
        display: flex;
        justify-content:center;
        align-items: center;
        height:30%;
        background-color: $woodsmoke;
        .img {
            filter: invert(50%);
            padding: 0 60px;
            img {
                width: 100px;
            }
        }
    }
}

</style>