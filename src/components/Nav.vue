<template>
  <div>
    <div class="top">
      <div class="opening-info">
          <i class="fas fa-clock"></i>
          <span>
            Open Hours: Mon - Sat - 9:00 - 18:00
          </span>
      </div>
      <div class="contacts-info">
        <div class="inner-info">
          <i class="fas fa-phone-alt"></i>
        <span>
          +1 (305) 1234-5678
        </span>
        </div>
        <div class="inner-info">
          <i class="fas fa-envelope"></i>
        <span>
          hello@example.com
        </span>
        </div>
        <i class="fab fa-facebook-f"></i>
        <i class="fab fa-twitter"></i>
        <i class="fab fa-linkedin-in"></i>
      </div>
    </div>
    <div class="sticky">
      <img :src="require(`../assets/img/logo.png`)" alt="logo Nex Gen">
      <div class="nav">
        <span>
          home
        </span>
        <span>
          services
        </span>
        <span>
          about
        </span>
        <span>
          projects
        </span>
        <span>
          results
        </span>
        <span>
          get in touch
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Nav'

}
</script>

<style lang="scss" scoped>
@import '../assets/Style/brandColors.scss';
.top {
  background-color: #21333E;
  height: 50px;
  color: $pumice;
  display: flex;
  justify-content: space-between;
  align-items: center;
  .opening-info {
    margin-left: 20%;
    i {
      padding-right: .5rem;
    }
  }
  .contacts-info {
    margin-right: 20%;
    display:flex;
    .inner-info i{
      padding: 0 10px;
    }
    i,
    .inner-info {
      padding: 0 1rem;
    }
  }
  
}
.sticky {
    position: sticky;
    top: 0;
    display:flex;
    width: 80%;
    margin: 0 auto;
    justify-content: space-around;
    align-items: center;
    padding-top: 20px;
    img {
      width:140px;
    }
    .nav {
      text-transform: uppercase;
      & span:last-child {
        background-color: $blueLagoon;
        padding: 15px 25px;
        border-radius: .3rem;
        color: $white;
        font-weight: 500;
      }
      span {
        padding:0 10px ;
      }
    }
  }

</style>