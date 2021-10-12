<template>
  <section id="searchBar">
    <hr>
    <div class="input-box">
      <img src="../../assets/icons/search-gray.svg" alt="">
      <input type="text" placeholder="search">
    </div>
  </section>
</template>

<script>

export default {
  name: 'searchBar'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

#searchBar{
  hr{
    border-top: 1px solid $c-bw-1;
    margin-bottom: 20px;
  }
  input{
    width: 100%;
    height: 40px;
    border: 2px solid $c-bw-1;
    border-radius: 5px;
    padding-left: 35px;
    @include corpo;
  }
  .input-box{
    position: relative;
    img{
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      left: 10px;
      height: 15px;
    }
  }
}

</style>
