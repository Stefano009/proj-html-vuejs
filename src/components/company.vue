<template>
  <div class="wrapper">
      <div class="left">
            <div class="row">
                    <h3>
                        about the network
                    </h3>
                    <h1>
                        <span>The</span> Company
                    </h1>
                    <p>
                        For 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and related services to select clients.
                    </p>
            </div>
            <div class="mini-card">
                <div class="row-card">
                    <i class="fas fa-award"></i>
                <h2>
                    tradition
                </h2>
                </div>
                <p>
                    Lorem ipsum dolor sit amet,<br> consectetur adipiscing elit. 
                </p>
            </div>
            <div class="mini-card">
                <div class="row-card">
                    <i class="fas fa-lock"></i>
                <h2>
                    security
                </h2>
                </div>
                <p>
                    Lorem ipsum dolor sit amet,<br> consectetur adipiscing elit. 
                </p>
            </div>
            <div class="mini-card">
                <div class="row-card">
                    <i class="far fa-edit"></i>
                <h2>
                    certificate
                </h2>
                </div>
                <p>
                    Lorem ipsum dolor sit amet,<br> consectetur adipiscing elit. 
                </p>
            </div>
            <div class="mini-card">
                <div class="row-card">
                    <i class="fas fa-graduation-cap"></i>
                <h2>
                    expertise
                </h2>
                </div>
                <p>
                    Lorem ipsum dolor sit amet,<br> consectetur adipiscing elit. 
                </p>
            </div>
            <div class="row-btn">
                <div class="btn-left">
                    <span>GET IN TOUCH</span>
                </div>
                <div class="btn-right">
                    <span> READ MORE</span>
                </div>
            </div>
        </div>
      <div class="right">
          <img src="../assets/img/about-4.jpg" alt="">
      </div>
  </div>
</template>

<script>
export default {
    name: 'company',
}
</script>

<style lang="scss" scoped>
@import '../assets/Style/brandColors.scss';
.wrapper {
    height: 90vh;
    width: 100%;
    background-color: $woodsmoke;
    display: flex;
    .left, 
    .right {
        width: 50vw;
    }
    .right img {
        height:100%;
        max-width: 50vw;
    }
    .left {
        color: $white;
        display: flex;
        flex-wrap: wrap;
        padding-left: 20vw;
        .row {
            padding-top: 25%;
            h3 {
                color: lighten($elm, 5%);
                text-transform: uppercase;
                font-size: 0.8rem;
            }
            h1 {
                padding: 30px 0;
                font-size: 4rem;
                span {
                    background-color: rgba($elm, .2);
                    padding: 10px;
                }
            }
            p {
                color: $pumice;
                font-size: 1.4rem;
            }
        }
        
        .mini-card {
            padding:20px;
            .row-card {
                display: flex;
                justify-content: flex-start;
                align-items: center;
                padding-bottom: 30px;
            }
            h2 {
                text-transform: capitalize;
                font-size: 1.8rem;
            }
            i {
                font-size: 2rem;
                color: $elm;
                padding-right: 10px;
            }
            p {
                font-size: 1.4rem;
                color: $pumice;           
              }
        }
        .row-btn {
                display: flex;
                width: 100%; 
                .btn-left,
                .btn-right {
                    margin:40px 40px 200px;
                    font-size:1.4rem;
                }
                .btn-left span{
                    background-color:$elm;
                    padding: 15px;
                    border-radius: .3rem;
                }
                .btn-right span{
                    padding: 15px;
                    border-radius: .3rem;
                    border: 1px solid $elm;
                }
            }
        
    }
}
</style>