<template>
  <footer>
    <!-- Footer Hero -->
    <FooterHero/>

    <!-- Footer -->
    <div class="f-imgs">
      <div><img src="../assets/images/Yogurt-Nan.jpg" alt=""></div>
      <div><img src="../assets/images/Mixed-fruits.jpg" alt=""></div>
      <div><img src="../assets/images/r-rachel-park-366508-unsplash-min.jpg" alt=""></div>
      <div><img src="../assets/images/r-michelle-tsang-500721-unsplash-min.jpg" alt=""></div>
    </div>

    <div class="f-top">
      <div class="container">
        <div class="block">
          <img class="logo" src="../assets/images/avada-food-logo-mob-2x.png" alt="avada food logo">
          <ul class="social">
            <li><a href="https://www.facebook.com/" target="_blank">
              <img src="../assets/icons/facebook.svg" alt="Facebook logo">
            </a></li>
            <li><a href="https://www.instagram.com/" target="_blank">
              <img src="../assets/icons/instagram.svg" alt="Instagram logo">
            </a></li>
            <li><a href="https://www.twitter.com/" target="_blank">
              <img src="../assets/icons/twitter.svg" alt="Twitter logo">
            </a></li>
            <li><a href="https://www.youtube.com/" target="_blank">
              <img src="../assets/icons/youtube.svg" alt="YouTube logo">
            </a></li>
            <li><a href="https://www.pinterest.com/" target="_blank">
              <img src="../assets/icons/pinterest.svg" alt="Pinterest logo">
            </a></li>
          </ul>
        </div>
        <div class="block">
          <ul>
            <li><a href="">Recipes</a></li>
            <li><a href="">Places</a></li>
            <li><a href="">Blog</a></li>
            <li><a href="">About</a></li>
            <li><a href="">Contact</a></li>
          </ul>
        </div>
        <div class="block">
          <h3>Contact</h3>
          <ul class="businessC">
            <li>
              <img src="../assets/icons/location.svg" alt="address icon">
              775 New York Ave, Brooklyn, Kings, New York 11203
            </li>
            <li>
              <img src="../assets/icons/phone.svg" alt="phone icon">
              +0100-505-0000
            </li>
            <li>
              <img src="../assets/icons/mail.svg" alt="mail icon">
              info@your-domain.com
            </li>
          </ul>
        </div>
        <div class="block" id="dwnApp">
          <h3>Get our App!</h3>
          <img src="../assets/images/download-app-store.png" alt="Click to download our app from GooglePlay">
          <img src="../assets/images/download-app-store.png" alt="Click to download our app from AppStore">
        </div>
      </div>
    </div>

    <div class="f-bottom">
      <p>© Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All rights Reserved | Powered by Wordpress</p>
      <a href="#" class="BackToTop">
        <img src="../assets/icons/arrow-up.svg" alt="arrow up icon">
      </a>
    </div>

  </footer>
</template>

<script>
import FooterHero from './FooterHero.vue'
export default {
  name: 'Footer',
  components:{
    FooterHero,
  }
  // props: {
  //   msg: String
  // }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

footer{
  margin-top: 40px;
}
.container{
  display: flex;
}

.f-imgs{
  display: flex;
  img{
    @include fit-cover;
  }
}

.f-top{
  padding: 30px 0;
  background-color: $white;

  .block{
    width: calc(100% / 4);
    padding: 15px 25px;
    border-right: 1px solid $c-bw-1;

    &:last-child{
      border-right: none;
    }
  }

  ul{
    list-style: none;
    li{
      margin-top: 15px;
      color: $text-gray;
      @include corpo;
      font-size: .8125rem;
    }
    a{
      color: $text-black;
      text-decoration: none;
      font-size: 1rem;
    }
  }
  ul.businessC{
    li{
      display: flex;
      align-items: center;
    }
    img{
      width: .9375rem;
      margin-right: 10px;
    }
  }
  ul.social{
    margin-top: 15px;
    li{
      display: inline-block;
      margin-right: 10px;
    }
    img{
      width: 1.2rem;
      margin-right: 10px;
    }
  }

  h3{
    @include title4;
    color: $c-main;
    font-size: 1.125rem;
    padding-bottom: 10px;
  }
}
img.logo{
  width: 100%;
}
#dwnApp img{
  width: 70%;
  margin-top: 10px;
  cursor: pointer;
}


.f-bottom{
  height: 60px;
  @include flex-center;
  @include corpo;
  position: relative;
  margin: 15px 0;

  a.BackToTop{
    @include flex-center;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    left: 30px;

    height: 50px;
    width: 50px;
    border-radius: 50%;
    background-color: $c-bw-3;

    img{
      width: 48%;
    }
  }
}

</style>
