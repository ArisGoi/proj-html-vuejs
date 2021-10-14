<template>
  <section id="twitterBox">
    <div class="title-row">
      <h3>Tweets <span>by</span> <a href="">@Theme_Fusion</a></h3>
      <img src="../../assets/icons/info.svg" alt="">
    </div>
    <div class="content-row">
      <div>
        <img src="../../assets/images/3a74ce3d0532b7773b174c45ca3bd05a_bigger.png" alt="profile icon" class="profile-i">
      </div>
      <div>
        <h4>Theme Fusion</h4>
        <a href="">@Theme_Fusion</a>
        <p>
          Do you need a sublime WordPress hosting for your next website? Take advantage of exclusive partner offers that we have secured just for you, & launch your site in seconds with <a href="https://twitter.com/search?q=%23avada&src=typed_query&f=live" target="_blank">#avada</a> on WP Engine hosting & get 30% Off this Black Friday <a href="bit.ly/3kjLLE2" target="_blank">bit.ly/3kjLLE2</a> <a href="https://twitter.com/search?q=%23blackfriday2020" target="_blank">#BlackFriday2020</a>
        </p>
        <img src="../../assets/icons/twitter-light.svg" alt="">
      </div>
    </div>
    <div class="img-box">
      <img src="../../assets/images/En2TRxLW4AEiWUN.jpeg" alt="">
    </div>
    <div class="actions-row">
      <button>
        <img src="../../assets/icons/love.svg" alt="love icon">
      </button>
      <button>
        <img src="../../assets/icons/share.svg" alt="share icon">
      </button>
      <span>21h</span>
    </div>
  </section>
</template>

<script>

export default {
  name: 'twitterBox'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

#twitterBox{
  width: 100%;
  margin-top: 30px;
  border-radius: 15px;
  padding: 20px;
  background-color: $white;

  a{
    text-decoration: none;
    color: rgb(33, 122, 177);
  }
}
.title-row{
  position: relative;
  h3{
    @include sans400;
    font-size: 1.375rem;
  }
  span, a{
    font-size: 12px;
    color: $text-gray;
  }
  img{
    position: absolute;
    top: 50%;
    right: 10px;
    transform: translateY(-50%);
    cursor: pointer;
  }
}
.content-row{
  display: flex;
  margin-top: 15px;
  @include sans400;
  position: relative;

  div:first-child{
    margin-right: 10px;
    img{
      max-width: 35px;
    }
  }
  div:last-child img:last-child{
    height: 25px;
    width: 25px;
    position: absolute;
    top: 0;
    right: 10px;
  }
  h4{
    @include sans600;
    font-size: 1.0625rem;
  }
}
.img-box{
  width: 100%;
  overflow: hidden;
  border-radius: 10px;
  margin-top: 20px;
  img{
    @include fit-cover;
  }
}
.actions-row{
  margin: 10px 0;
  display: flex;
  span{margin-left: auto; color: $text-gray;}
  button{
    margin-right: 10px;
    background-color: transparent;
    border: none;
    padding: 1px;
    cursor: pointer;
    img{
      width: 1.125rem;
      height: 1.125rem;
    }
  }
}

</style>
