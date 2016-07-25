<template>
  <div class="evaluate-nav">
    <div class="evaluate-result-container">
      <div class="nav-list">
        <div class="item">匹配结果</div>
        <div class="item iconfont  icon-dian-copy point"></div>
        <div class="item sprint-collage active">冲刺院校 (2)</div>
        <div class="item core-collage">核心院校 (6)</div>
      </div>
    </div>
  </div>
</template>

<script>
  export default{
    props: {
      coreCollage: {},
      sprintCollage: {}
    },
    components: {}
  }
</script>

<style scoped lang="stylus">
  @import '../assets/stylus/variables.styl'

  .evaluate-nav {
    height $evaluateNavHeight+$headerHeight
    background #ffffff;
    display flex
    align-items flex-end
    justify-content space-around
  }

  .evaluate-result-container {
    height $evaluateNavHeight;
    width 3.50rem
    display flex
    align-items stretch
    justify-content center
  }

  .nav-list {
    display flex;
    .item {
      line-height $evaluateNavHeight;
      &.active {
        color #0e2e61
        border-bottom .03rem solid #0e2e61;
      }
      margin 0 0.05rem 0 0.1rem
      &.point {
        font-weight 700
        padding-top 0.015rem
        margin 0 0.01rem
      }
      &.sprint-collage {
        margin 0 0.05rem
      }
      &.core-collage {
        margin 0 0.1rem 0 0.05rem
      }
      justify-content space-between
      font-size 0.14rem
    }
  }

  .active {
    color #0e2e61
  }

  .collage-name-cn {
    color: #0e2d60
  }
</style>
