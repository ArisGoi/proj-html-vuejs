<template>
  <section id="popularRecipes">
      <div class="container">

          <sectionHeadline title="Popular Recipes" subtitle="Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis."/>

          <div class="content">

              <div class="big-recipe">
                  <div class="img">
                    <img src="../../assets/images/Yogurt-Nan.jpg" alt="">
                    <div class="hover-img-link">
                        <img src="../../assets/icons/link.svg" alt="">
                        <p>Lunch Favorite with Salad, Naan and Beans</p>
                    </div>
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
                <div>
                    <img src="../../assets/images/Mixed-fruits.jpg" alt="">
                    <div class="hover-img-link">
                        <img src="../../assets/icons/link.svg" alt="">
                        <p>Fruit Platter with Banana, Mango, Berries and Orange</p>
                    </div>
                </div>
                <div>
                    <img src="../../assets/images/r-rachel-park-366508-unsplash-min.jpg" alt="">
                    <div class="hover-img-link">
                        <img src="../../assets/icons/link.svg" alt="">
                        <p>Beautiful breakfast of my dreams</p>
                    </div>
                </div>
                <div>
                    <img src="../../assets/images/r-michelle-tsang-500721-unsplash-min.jpg" alt="">
                    <div class="hover-img-link">
                        <img src="../../assets/icons/link.svg" alt="">
                        <p>Magic Icecreams balls: chocolate's secret</p>
                    </div>
                </div>
                <div>
                    <img src="../../assets/images/quick-summer-drink-460x295.jpg" alt="">
                    <div class="hover-img-link">
                        <img src="../../assets/icons/link.svg" alt="">
                        <p>Top 10 Best Summer Cocktails</p>
                    </div>
                </div>
                <div>
                    <img src="../../assets/images/r-maarten-van-den-heuvel-400626-unsplash-min-460x295.jpg" alt="">
                    <div class="hover-img-link">
                        <img src="../../assets/icons/link.svg" alt="">
                        <p>Vegetables is the future</p>
                    </div>
                </div>
                <div>
                    <img src="../../assets/images/perfect-cosmopolitan-460x295.jpg" alt="">
                    <div class="hover-img-link">
                        <img src="../../assets/icons/link.svg" alt="">
                        <p>Love drinks list</p>
                    </div>
                </div>
                <div>
                    <img src="../../assets/images/fi2x-6-460x295.jpg" alt="">
                    <div class="hover-img-link">
                        <img src="../../assets/icons/link.svg" alt="">
                        <p>Heathy food ever</p>
                    </div>
                </div>
                <div>
                    <img src="../../assets/images/r-brooke-lark-96398-unsplash-min-460x295.jpg" alt="">
                    <div class="hover-img-link">
                        <img src="../../assets/icons/link.svg" alt="">
                        <p>Sweet Morning with your Partner</p>
                    </div>
                </div>
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
            position: relative;

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
        & > div{
            position: relative;
            height: 165px;
            width: calc(50% - 15px);
            img{@include fit-cover}
        }
    }
}

</style>
