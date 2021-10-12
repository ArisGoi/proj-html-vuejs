<template>
  <section id="socialBox">
    <h4>Follow Us</h4>

    <div class="icons-container">
      <a class="icon-box" href="https://www.facebook.com/" target="_blank">
        <img src="../../assets/icons/facebook.svg" alt="Facebook logo">
      </a>
      <a class="icon-box" href="https://www.instagram.com/" target="_blank">
        <img src="../../assets/icons/instagram.svg" alt="Instagram logo">
      </a>
      <a class="icon-box" href="https://www.twitter.com/" target="_blank">
        <img src="../../assets/icons/twitter.svg" alt="Twitter logo">
      </a>
      <a class="icon-box" href="https://www.youtube.com/" target="_blank">
        <img src="../../assets/icons/youtube.svg" alt="YouTube logo">
      </a>
      <a class="icon-box" href="https://www.pinterest.com/" target="_blank">
        <img src="../../assets/icons/pinterest.svg" alt="Pinterest logo">
      </a>
    </div>
  </section>
</template>

<script>

export default {
  name: 'socialBox'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

#socialBox{
  margin-top: 30px;
  h4{
    @include title5;
    color: $c-main;
    margin-bottom: 15px;
  }
  .icons-container{
    display: flex;
    .icon-box{
      width: 40px;
      height: 40px;
      margin-right: 10px;
      border-radius: 8px;
      border: 1px solid $c-bw-1;
      background-color: $c-bw-4;
      @include flex-center;
      padding: 8px;
    }
  }
}

</style>
