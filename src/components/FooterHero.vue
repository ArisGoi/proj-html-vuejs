<template>
  <div id="footer-hero">
    <div class="container">
      <h2>Subscribe <span>&</span> Receive A Free eBook</h2>
      <p>Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.</p>
      <div class="inputMail">
        <input type="email" name="inputEmail" id="inputEmail" placeholder="Insert your email _*">
        <button class="btn-1">Subscribe</button>
      </div>
      <p>Cras portittor pellentesque sem eu pretium</p>
    </div>

  </div>
</template>

<script>
export default {
  name: 'FooterHero',
  // props: {
  //   msg: String
  // }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

#footer-hero{
  min-height: 600px;
  background-color: $white;
  position: relative;
  background-image: url(../assets/images/subscribe-sec-bg.png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;

  .container{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    @include flex-col-center;
  }

  h2{
    @include title3;
    span{color: $c-main}
    color: $text-black;
  }
  p{
    @include corpo;
    margin: 20px 0 40px 0;
  }

  input{
    height: 38px;
    min-width: 300px;
    border: 2px solid $c-bw-1;
    padding: 15px;
    flex-grow: 1;
    margin-right: 20px;
  }
}

</style>
