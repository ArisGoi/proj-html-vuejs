<template>
  <div class="card-small">
    <div class="img">
      <img :src="require(`../../assets/images/${img}`)" alt="">
      <div class="hover-img-link">
        <img src="../../assets/icons/link.svg" alt="">
        <p>{{title}}</p>
      </div>
    </div>
    <div class="text">
      <h3>{{title}}</h3>
      <p>{{authorDate}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'cardSmall',
  props: ['img','title','authorDate'],
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

.card-small{
  background-color: $white;
  max-width: 350px;
}

.text{
  padding: 20px;
  text-align: center;
}

.img{
  width: 100%;
  height: 230px;
  overflow: hidden;
  position: relative;

  img{
    @include fit-cover;
  }
}

h3{
  @include title5;
  margin-bottom: 10px
}
p{
  @include corpo;
}

</style>
