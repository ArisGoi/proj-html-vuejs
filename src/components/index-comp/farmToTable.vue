<template>
  <section id="farmToTable">
      <div class="container">

        <div class="headline">
            <h2>Farm to Table</h2>
            <h5>Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.</h5>

            <button class="btn-1">
                Read our blog
                <img src="../../assets/icons/blog.svg" alt="">
            </button>
        </div>

        <div class="content">
            <!-- LEFT SIDE -->
            <div class="side-left">

                <div class="big-article">
                    <div class="img">
                      <img src="../../assets/images/Yogurt-Nan.jpg" alt="">
                  </div>
                  <div class="body">
                      <h3>Food Corner: Top Japanese Restaurant for Sushi</h3>
                      <h5>By admin | March 25th, 2019</h5>
                      <div class="hr"></div>
                      <p>Suspendisse at semper odio. Nam fringilla scelerisque tincidunt. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec tincidunt posuere ornare. Phasellus placerat odio non feugiat sollicitudin. Integer vita elementum ex.</p>
                  </div>
                  <div class="more-bar">
                      <a href="">Read More ></a>
                      <img src="../../assets/icons/chat.svg" alt="">
                      <span>0</span>
                  </div>
                </div>

                <cardSmall img="single-post-img3.jpg" title="Food Corner: Top Japanese Restaurants for Sushi" authorDate="By admin | March 25th, 2019"/>
                <cardSmall img="single-post-img3.jpg" title="Food Corner: Top Japanese Restaurants for Sushi" authorDate="By admin | March 25th, 2019"/>
                <cardSmall img="single-post-img3.jpg" title="Food Corner: Top Japanese Restaurants for Sushi" authorDate="By admin | March 25th, 2019"/>
                <cardSmall img="single-post-img3.jpg" title="Food Corner: Top Japanese Restaurants for Sushi" authorDate="By admin | March 25th, 2019"/>
                <cardSmall img="single-post-img3.jpg" title="Food Corner: Top Japanese Restaurants for Sushi" authorDate="By admin | March 25th, 2019"/>
                <cardSmall img="single-post-img3.jpg" title="Food Corner: Top Japanese Restaurants for Sushi" authorDate="By admin | March 25th, 2019"/>

                <button class="btn-2">Load More Posts</button>
            </div>
            <!-- RIGHT SIDE -->
            <div class="side-right">

                <div class="adv-1">
                    <img src="../../assets/images/ad-bg.jpg" alt="background image of adv about our latest ecipes">
                    <p>View our latest recipe</p>
                </div>

                <div class="adv-2">
                    <img src="../../assets/images/singapore-featured-image.jpg" alt="background image of adv about Singapore - City Guide">
                    <button class="btn-1">
                        <img src="../../assets/icons/world.svg" alt="">
                        View all city guides
                    </button>
                </div>

                <!-- Search Bar -->
                <searchBar/>

                <!-- Social Box -->
                <socialBox/>
            </div>
        </div>

      </div>
  </section>
</template>

<script>
import cardSmall from './cardSmall.vue'
import searchBar from './search.vue'
import socialBox from './socialBox.vue'

export default {
  name: 'farmToTable',
  components:{
      cardSmall,
      searchBar,
      socialBox,
  },
  // props: {
  //   msg: String
  // }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

.headline{
    position: relative;
    margin: 85px 0px 35px 0px;
    h2{
        @include title4;
        margin-bottom: 26px;
    }
    h5{
        @include corpo;
        max-width: 550px;
    }
    .btn-1{
        position: absolute;
        top: 0;
        right: 0;
    }
}

.content{
    display: flex;
    justify-content: space-between;
}

.side-left{
    width: calc(65% - 10px);
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;

    div{
        margin-top: 30px;
        &:first-child{
            margin-top: 0px;
        }
    }

    .big-article{
        width: 100%;
        background-color: $white;

        .img{
            width: 100%;
            height: 500px;
            img{ @include fit-cover; }
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
            h5, p{ @include corpo; }
            button{
                cursor: pointer;
                margin-top: 25px;
            }
        }

        .more-bar{
            text-align: right;
            padding: 0 30px 30px 30px;
            a{
                text-decoration: none;
                color: $text-black;
                float: left;
                @include corpo;
            }
            img{ height: 18px; }
            span{
                @include corpo;
                margin-left: 5px;
            }
        }
    }

    .btn-2{
        width: 100%;
        margin-top: 30px;
    }
}

.side-right{
    width: calc(35% - 20px);

    .adv-1, .adv-2{
        width: 100%;
        margin-bottom: 40px;
        position: relative;
        & > img{
            @include fit-cover;
            display: block;
        }
    }
    .adv-1 p{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        max-width: 40%;
        @include title4;
        text-align: center;
    }
    .adv-2{
        button{
            width: 100%;
        }
        &::after{
            content: 'City guide: Singapore';
            color: white;
            background-color: black;
            padding: 10px;
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            left: 0;

            @include sans600;
            font-size: 1.375rem;
        }
    }
}

</style>
