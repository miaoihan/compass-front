<template>
  <div class="evaluate-nav-item">
    <div class="item-container">
      <div class="collage"></div>
      <div class="grade"></div>
    </div>
  </div>
</template>

<script>
  export default{
    components: {}
  }
</script>

<style scoped lang="stylus">

  .evaluate-nav-item {
    background-color #fff;
    width 100%;
    height 1.75rem;
    margin .1rem 0;
    .collage{
      width 100%;
      height 0.8rem
      border-bottom  1px solid #ebebeb;
    }
    .grade{
      height 0.4rem
      width 100%;
      border-bottom  1px solid #ebebeb;
    }
  }

  .item-container {
    margin 0 auto;
    width 3.50rem
    height 100%

  }

</style>
