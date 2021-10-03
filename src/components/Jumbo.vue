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
    </div>
</template>

<script>
export default {
    name: 'Jumbo',
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
}


</style>