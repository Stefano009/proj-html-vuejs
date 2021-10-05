<template>
<div class="wrapper">
    <div class="left">
        <div class="row">
            <h3>
            send a message
            </h3>
            <h1>
                Get in <span>Touch</span>
            </h1>
            <p>
                We will respond to your message as soon as possible.
            </p>
        </div>
        <div class="square">
            <form>
                <div class="labelled">
                    <input type="text" id="fname" name="fname" placeholder="Name">
                    <label for="fname">
                        <img src="../assets/img/image (1).png" alt="">
                    </label>
                </div>
                <input type="email" id="email" name="email" placeholder="Email">
                <input type="tel" id="phone" name="phone" placeholder="Phone">
                <div class="labelled">
                <input type="info" id="info" name="info" placeholder="More Info">
                <label for="info">
                    <i class="fas fa-angle-down"></i>
                </label>
                </div>
                <textarea name="text" id="text" cols="50" rows="7" placeholder="Message"></textarea>
                <div class="btn">
                    send
                </div>
            </form> 
        </div>
    </div>
    <div class="rigth">
        <h3>
            Example Inc.
        </h3>
        <p>
            Lorem ipsum dolor sit amet, consectetur<br> adipiscing elit.
        </p>
        <p>
            Praesent diam Iacus, dapibus sed imperdiet <br> consectetur.
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
            Main Avenue, 987
        </span>
        <div class="btn">
                VIEW MAP
        </div>
    </div>
    <div class="right">

    </div>
</div>
</template>

<script>
export default {
    name:'Form',

}
</script>

<style lang="scss" scoped>
@import '../assets/Style/brandColors.scss';
    .wrapper {
        width: 100vw;
        height: 90vh;
        display: flex;
        .left {
            width: 60%;
            padding: 100px 0 0 260px;
            .row {
                display: flex;
                flex-direction:column;
                padding-bottom: 50px;
                h3 {
                color: lighten($blueLagoon, 10%);
                text-transform: uppercase;
                } 
                h1 {
                    padding: 20px 0;
                    font-size: 3.7rem;
                    font-weight: 900;
                    span {
                        color: $blueLagoon;
                        background-color: rgba($blueLagoon, .2);
                        padding:0 10px;
                    }
                }
                p {
                    color: darken($pumice, 20%);
                    font-size: 1.3rem;
                }
            }
            .square {
                display: flex;
                flex-wrap: wrap;
                input {
                    margin: 10px;
                    width: 380px;
                    height: 50px;
                    background-color: rgba($pumice, 0.3);
                    border: none;
                    font-size: 1rem;
                    padding: 20px;
                    border-radius: .3rem;
                }
                .labelled {
                    display: inline-block;
                    position: relative;
                }
                label {
                    position: absolute;
                    top: 50%;
                    right:5%;
                    transform:translateY(-50%)
                }
                textarea {
                    margin: 10px;
                    width: 780px;
                    background-color: rgba($pumice, 0.3);
                    border: none;
                    font-size: 1rem;
                    padding: 20px;
                    border-radius: .3rem;
                    box-decoration-break: none;
                }
                .btn {
                    margin: 30px 10px;
                    height:50px;
                    width: 100px;
                    color: $white;
                    background-color: $blueLagoon;
                    font-size: 1.3rem;
                    border-radius: .3rem;
                    padding: 13px 20px;
                    text-transform: uppercase;
                    cursor: pointer;
                    
                }
            }
        }
        .rigth {
            width: 40%;
            padding-top: 100px;
            h3 {
               font-size: 1.5rem;    
               padding:20px 0;             
            }
            p  {
                font-size: 1rem;
                color: darken($pumice, 20%);
                padding: 20px 0;
            }
            span {
                font-size: 1.2rem;
                color: $blueLagoon;
                display:block;
                padding: 15px 0;
                i { 
                    background-color: rgba($blueLagoon, .1);
                    border-radius: 50%;
                    padding:15px;
                }
            }
            .btn {
                height:40px;
                width: 140px;
                border:1px solid $blueLagoon;
                border-radius: .3rem;
                padding: 10px 10px 10px 30px;
                color:$blueLagoon;
            }
        }
    }
</style>