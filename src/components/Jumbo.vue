<template>
    <div>
        <div class="center-item">
            <div class="row">
                <h1> Ready </h1>
                <h1 class="color-title">Team</h1>
            </div>
            <p>No matter what your company needs, we will be ready to assist you in the best possible way.</p>
            <div class="outer-btn">
                <div class="btn full">
                <span>
                    get in touch
                </span>
            </div>
            <div class="btn void">
                <span>
                    read more
                </span>
            </div>
            </div>
        </div>
        <div class="position">
            <div class="slider"></div>
            <div class="full slider"></div>
            <div class="slider"></div>
        </div>
        <div v-for="(position, index) in positions" class="square" :key="index" :style="position">
        </div>
    </div>
</template>

<script>
export default {
    name: 'Jumbo',
    data(){
        return{
            positions: [
                'top: 5%; left: 5%',
                'top: 10%; left: 10%',
                'top: 23%; left: 23%',
                'top: 60%; left: 60%',
                'top: 98%; left: 98%',
                'top: 23%; left: 32%',
                'top: 21%; left: 54%',
                'top: 26%; left: 32%',
                'top: 10%; left: 6%',
                'top: 52%; left: 4%',
                'top: 21%; left: 18%',
                'top: 34%; left: 6%',
                'top: 10%; left: 62%',
                'top: 10%; left: 3%',
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/Style/brandColors.scss';
div{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 80%;
    position: relative;
    .slider {
        height:35px;
        width:8px;
        border: 1px solid $blueLagoon;
        margin: 5px;
        border-radius: .3rem;
    }
    .position {
        position: absolute;
        top: 10%;
        right:10px;
    }
    .center-item {
        height:10vh;
        .row {
            display:flex;
            flex-direction: row;
            font-size: 2.3rem;
            h1 {
                font-weight: 900;
            }
        }
        p {
            width: 450px;
            padding: 30px 15px;
            font-size: 1.2rem;
            text-align: center;
            color: gray;
        }
        .btn {
            font-size:1.1rem;
            text-transform: uppercase;
        }
        .full {
            background-color: $blueLagoon;
            padding: 15px 20px;
            border-radius: .3rem;
            color: $white;
        }
        .void {
            margin-left: 15px;
            padding: 15px 20px;
            border-radius: .3rem;
            color: $blueLagoon;
            border: 1px solid $blueLagoon;
        }
        .outer-btn {
            display: flex;
            flex-direction: row;
            justify-content:space-around;
        }
    }
    .square {
        width: 100px;
        height: 100px;
        background-color:rgba($pumice, .4);
        position:absolute;
        z-index: -1;
    }
}


</style>