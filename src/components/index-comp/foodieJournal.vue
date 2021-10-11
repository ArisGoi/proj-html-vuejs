<template>
<div class="container">
  <section id="foodieJournal">

    <div class="headline">
    <div class="hr"></div>
    <h2>Foodie Journal</h2>
    </div>
    <div class="content">
      <!-- Vanno sostituiti gli elementi in "content" con una <CARD/> -->
      <div class="segnaposto" style="height:100px; width:80px; background-color: blue"></div>
      <div class="segnaposto" style="height:100px; width:80px; background-color: blue"></div>
      <div class="segnaposto" style="height:100px; width:80px; background-color: blue"></div>
    </div>

  </section>
</div>
</template>

<script>
export default {
  name: 'foodieJournal',
  // props: {
  //   msg: String
  // }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

#foodieJournal{
  top: -70px;
  position: relative;
  padding: 30px;
  background-color: $white;
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
