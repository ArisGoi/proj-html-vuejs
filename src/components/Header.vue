<template>
  <header>
    <div class="top">
      <img src="../assets/images/avada-food-logo-2x.png" alt="">
    </div>

    <nav class="nav">
      <ul>
        <li class="current">Home</li>
        <li>Recipes</li>
        <li>Places</li>
        <li>Blog</li>
        <li>About</li>
        <li>Contact</li>
        <li><img src="../assets/icons/search.svg" height="15" alt=""></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  // props: {
  //   msg: String
  // }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

header{
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 10;

  .top{
    background-color: $white;
    height: 150px;
    padding: 10px;
    @include flex-center;

    img{
      height: 100%;
    }
  }

  .nav{
    background-color: $white;
    height: 65px;

    ul{
      list-style: none;
      @include flex-center;
      height: 100%;

      li{
        @include sans600;
        cursor: pointer;
        padding: 0 20px;
        color: $nav-text;
        font-size: 1.08rem;

        &.current{
          color: $c-main;
          position: relative;
          &::after{
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            height: 3px;
            width: calc(100% - 40px);
            background-color: $c-main;
          }
        }
      }
    }
  }
}

</style>
