<template>
    <div>
        <div class="center-item">
            <div class="row">
                <h1> Ready </h1>
                <h1 class="item">Team</h1>
            </div>
            <p>No matter what your company needs, we will be ready to assist you in the best possible way.</p>
            <div class="btn">
                <span>
                    get in touch
                </span>
            </div>
            <div class="btn">
                <span>
                    read more
                </span>
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
            font-size: 2.5rem;
        }
        p {
            max-width: 350px;
            padding: 15px;
        }
    }
}


</style>