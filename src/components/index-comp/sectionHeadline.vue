<template>
    <div class="container">
        <div class="headline">
            <h2>{{title}}</h2>
            <h5>{{subtitle}}</h5>
        </div>
    </div>
</template>

<script>
export default {
  name: 'sectionHeadline',
  props:['title','subtitle'],
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/style.scss';

.container{
    max-width: 600px !important;
}

.headline{
    text-align: center;
    margin: 85px 0px 35px 0px;
    h2{
        @include title4;
        margin-bottom: 26px;
    }
    h5{
        @include corpo;
    }
}

</style>
