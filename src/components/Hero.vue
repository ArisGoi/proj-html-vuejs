<template>
  <section id="hero">

    <img src="../assets/images/single-post-img3.jpg" alt="">

    <div class="title-box">
      <div class="pick">Today's Pick</div>
      <h2>Food Corner: Top Japanese Restaurants for Sushi</h2>
      <h6>March 25, 2019</h6>
    </div>

  </section>
</template>

<script>
export default {
  name: 'Hero',
  // props: {
  //   msg: String
  // }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/style.scss';

#hero{
  width: 100%;
  height: 850px;
  background-color: lightblue;
  position: relative;

  img{
    height: 100%;
    width: 100%;
    object-fit: cover;
  }
}

.title-box{
  padding: 46px;
  text-align: center;
  position: absolute;
  top: calc(50% - 40px);
  left: 50%;
  transform: translate(-50%, -50%);
  background-color: $white;
  border-radius: 13px;
  max-width: 800px;

  .pick{
    @include title4;
    color: white;
    position: absolute;
    top: 0;
    left: 50%;
    transform: inherit;
    border-radius: inherit;
    background-color: $c-main;
    padding: 10px;
    font-size: 1.125rem;
  }

  h2{
    @include title2;
  }
  h6{
    @include subInfo;
    margin-top: 20px;
  }
}

</style>
