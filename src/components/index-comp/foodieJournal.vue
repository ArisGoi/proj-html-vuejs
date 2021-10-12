<template>
<div class="container">
  <section id="foodieJournal">

    <div class="headline">
      <div class="hr"></div>
      <h2>Foodie Journal</h2>
    </div>
    <div class="content">
      <cardSmall img="single-post-img3.jpg" title="Food Corner: Top Japanese Restaurants for Sushi" authorDate="By admin | March 25th, 2019"/>
      <cardSmall img="fi-roundup.jpg" title="Roundup: My New Favourite Recipes For Healthy Living" authorDate="By admin | March 25th, 2019"/>
      <cardSmall img="fi-toasts.jpg" title="Why These Toasts with Tea are My New Favorite" authorDate="By admin | March 25th, 2019"/>
    </div>

  </section>
</div>
</template>

<script>
import cardSmall from './cardSmall.vue'

export default {
  name: 'foodieJournal',
  components: {
    cardSmall,
  }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

#foodieJournal{
  top: -70px;
  position: relative;
  padding: 30px;
  background-color: $white;
  margin-bottom: -35px;
}

.headline{
  @include flex-center;
  padding-bottom: 30px;
  position: relative;

  .hr{
    height: 1px;
    width: 100%;
    background-color: $c-bw-1;
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
  }

  h2{
    @include title4;
    background-color: $white;
    z-index: 1;
    padding: 0 40px;
  }
}

.content{
  display: flex;
  justify-content: space-around;
}

</style>
