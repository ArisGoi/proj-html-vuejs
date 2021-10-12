<template>
  <section id="popularRecipes">
      <div class="container">

          <sectionHeadline title="Popular Recipes" subtitle="Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis."/>

          <div class="content">

              <div class="big-recipe">
                  <div class="img">
                      <img src="../../assets/images/Yogurt-Nan.jpg" alt="">
                  </div>
                  <div class="body">
                      <h3>Lunch Favourite with Salad, Naan And Beans</h3>
                      <h5>Bakery, Featured, Healthy, Latest Recipes, Staff Picks</h5>
                      <div class="hr"></div>
                      <p>Suspendisse at semper odio. Nam fringilla scelerisque tincidunt. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec tincidunt posuere ornare. Phasellus placerat odio non feugiat sollicitudin. Integer vita elementum ex. Sed porttitor. diam eget convallis volutpat, arcu tellus facilisis nulla, id dignissim orci leo id</p>

                      <button class="btn-1">Learn More</button>
                  </div>
              </div>

              <div class="others">
                  <img src="../../assets/images/Mixed-fruits.jpg" alt="">
                  <img src="../../assets/images/r-rachel-park-366508-unsplash-min.jpg" alt="">
                  <img src="../../assets/images/r-michelle-tsang-500721-unsplash-min.jpg" alt="">
                  <img src="../../assets/images/quick-summer-drink-460x295.jpg" alt="">
                  <img src="../../assets/images/r-maarten-van-den-heuvel-400626-unsplash-min-460x295.jpg" alt="">
                  <img src="../../assets/images/perfect-cosmopolitan-460x295.jpg" alt="">
                  <img src="../../assets/images/fi2x-6-460x295.jpg" alt="">
                  <img src="../../assets/images/r-brooke-lark-96398-unsplash-min-460x295.jpg" alt="">
              </div>

          </div>

      </div>
  </section>
</template>

<script>
import sectionHeadline from './sectionHeadline.vue'
export default {
  name: 'popularRecipes',
  components:{
      sectionHeadline,
  },
  // props: {
  //   msg: String
  // }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

.content > div{
    width: calc(50% - 20px);
}

.content{
    display: flex;
    justify-content: space-between;

    .big-recipe{
        background-color: $white;

        .img{
            width: 100%;
            height: 380px;

            img{
                @include fit-cover;
            }
        }
    }

    .body{
        padding: 40px 30px;
        .hr{
            height: 1px;
            width: 100%;
            background-color: $c-bw-1;
            margin: 20px 0;
        }

        h3{
            @include title5;
            margin-bottom: 8px;
        }

        h5, p{@include corpo;}

        button{
            cursor: pointer;
            margin-top: 25px;
        }
    }

    .others{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        align-content: space-between;
        img{
            height: 165px;
            width: calc(50% - 15px);
            object-fit: cover;
        }
    }
}

</style>
