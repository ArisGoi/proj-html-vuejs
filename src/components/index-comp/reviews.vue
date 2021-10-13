<template>
  <section id="reviews">

    <div class="selector">
      <button class="btn-extra active">Popular</button>
      <button class="btn-extra">Recent</button>
    </div>

    <ul class="review-list">
      <li>
        <div class="rnd-img">
          <img src="../../assets/images/single-post-img3.jpg" alt="">
        </div>
        <div class="text">
          <h5>Food Corner: Top Japanese Restaurants for Sushi</h5>
          <p>March 25th, 2019</p>
        </div>
      </li>

      <li>
        <div class="rnd-img">
          <img src="../../assets/images/singapore-featured-image.jpg" alt="">
        </div>
        <div class="text">
          <h5>City Guide: Singapore</h5>
          <p>February 27th, 2019</p>
        </div>
      </li>

      <li>
        <div class="rnd-img">
          <img src="../../assets/images/slide1-bg-150x150.jpg" alt="">
        </div>
        <div class="text">
          <h5>6 Nutritional Tips to Help Burn Body Fat</h5>
          <p>February 28th, 2019</p>
        </div>
      </li>
    </ul>
  </section>
</template>

<script>

export default {
  name: 'reviews'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

#reviews{
  margin-top: 35px;
}

.selector{
  width: 80%;
  margin: auto;
  @include flex-center;

  .btn-extra{
    @include title5;
    border: 2px solid $c-bw-4;
    background-color: $bg-body;
    font-size: 1.125rem;
    padding: 10px 45px;

    &.active{
      background-color: $white;
    }

    &:first-child{
      border-right-width: 1px;
    }
    &:last-child{
      border-left-width: 1px;
    }
  }
}

ul.review-list{
  list-style: none;
  width: 100%;
  @include sans300;
  color: $text-gray;
  h5{
    font-size: 1rem;
    font-weight: 300;
  }
  p{
    font-size: .8125rem;
  }

  li{
    margin-top: 20px;
    &:first-child{margin-top: 30px;}
    display: flex;
    align-items: center;

    .rnd-img{
      height: 50px;
      width: 50px;
      border-radius: 50%;
      margin-right: 10px;
      background-color: cadetblue;
      overflow: hidden;
      img{
        @include fit-cover;
      }
    }
  }
}


</style>
