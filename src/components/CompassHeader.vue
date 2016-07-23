<template>
  <div class="header">
    <img class="logo" src="../assets/logo.png">

    <button class="btn-clear toggle iconfont icon-toggle"></button>
  </div>
  <div class="header-fix"></div>
</template>

<script>
  export default{}
</script>

<style lang="stylus" scoped>
  $headerHeight = 0.44rem
  .header {
    position fixed
    margin 0 auto
    width 95%
    height $headerHeight;
    top 0;
    left 2.5%;
    background-color #1ddab0
    display flex
    justify-content space-between
    align-items center
    .logo {
      margin-left 0.1rem;
      width 0.97rem
      height 0.22rem
      display block
    }
  }

  .toggle {
    margin-right 0.1rem
    font-size 0.22rem;
  }

  .header-fix {
    height $headerHeight
  }
</style>
