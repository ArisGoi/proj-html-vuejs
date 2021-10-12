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
            
        </div>

      </div>
  </section>
</template>

<script>
export default {
  name: 'farmToTable',
  components:{
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

        img{
            height: 15px;
            transform: translateY(.125rem);
            margin-left: .3125rem;
        }
    }
}


</style>
