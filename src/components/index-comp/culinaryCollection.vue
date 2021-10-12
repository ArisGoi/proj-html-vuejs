<template>
  <section id="culinaryCollection">
      <div class="container">

          <sectionHeadline title="Culinary Collection" subtitle="Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis."/>

          <div class="content">
              <a href="" class="cc-card">
                  <div>
                      <img src="../../assets/images/drinks-recipes.png" alt="">
                  </div>
                  <h3>Drinks</h3>
              </a>
              <a href="" class="cc-card">
                  <div>
                      <img src="../../assets/images/soups-recipes.png" alt="">
                  </div>
                  <h3>Soups</h3>
              </a>
              <a href="" class="cc-card">
                  <div>
                      <img src="../../assets/images/baking-recipes.png" alt="">
                  </div>
                  <h3>Bakery</h3>
              </a>
              <a href="" class="cc-card">
                  <div>
                      <img src="../../assets/images/dinner-recipes.png" alt="">
                  </div>
                  <h3>Dinner</h3>
              </a>
              <a href="" class="cc-card">
                  <div>
                      <img src="../../assets/images/healthy-recipes.png" alt="">
                  </div>
                  <h3>Healthy</h3>
              </a>
              <a href="" class="cc-card">
                  <div>
                      <img src="../../assets/images/staff-picks.png" alt="">
                  </div>
                  <h3>Staff Picks</h3>
              </a>
              <a href="" class="cc-card">
                  <div>
                      <img src="../../assets/images/premium-recipes.png" alt="">
                  </div>
                  <h3>Appetisers</h3>
              </a>
              <a href="" class="cc-card">
                  <div>
                      <img src="../../assets/images/quick-easy-recipes.png" alt="">
                  </div>
                  <h3>Quick & easy</h3>
              </a>
          </div>

      </div>
  </section>
</template>

<script>
import sectionHeadline from './sectionHeadline.vue'
export default {
  name: 'culinaryCollection',
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

.content{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.cc-card{
    width: calc(100% / 4 - 24px);
    margin-bottom: 25px;
    padding: 20px 10px 10px 10px;

    background-color: $white;
    text-decoration: none;
    box-shadow: 0px 0px 12px 0px rgba(0,0,0,0.15);

    display: flex;
    flex-direction: column;
    align-items: center;

    img{
        height: 90px;
        margin-bottom: 15px;
    }

    h3{
        padding: 15px;
        width: 100%;
        text-align: center;
        @include title4;
        font-size: 1.05rem;
    }

    &:hover{
        h3{
            color: white;
            background-color: $c-main;
        }
    }
}

</style>
