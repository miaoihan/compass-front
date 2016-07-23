<template>
  <div class="header">
    <img v-if="showLogo" class="logo" src="../assets/logo.png">
    <a v-if="showLeftArrow" class="iconfont icon-left left-arrow"></a>
    <div v-if="title" class="title" v-if="title">{{title}}</div>
    <button v-if="showToggle" class="btn-clear toggle iconfont icon-toggle"></button>

  </div>
  <div v-if="needFixHeight" class="header-fix-height"></div>
</template>

<script>
  export default{
    props: {
      needFixHeight: {
        type: Boolean,
        default: true
      },
      showLogo: {
        type: Boolean,
        default: false
      },
      showLeftArrow: {
        type: Boolean,
        default: true
      },
      showToggle: {
        type: Boolean,
        default: false
      },
      title: {
        type: String,
        default: ''
      }

    }
  }
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
      margin-left 0.14rem;
      width 0.97rem
      height 0.22rem
      display block
    }
    .toggle {
      margin-right 0.14rem
      font-size 0.22rem;
    }
    .left-arrow {
      color: #fff;
      margin-left 0.14rem;
      font-size: .18rem;
    }
    .title {
      color #fff
      $fontSize = .18rem
      position: absolute
      line-height $headerHeight
      font-size $fontSize
      text-align center
      left 0
      right 0
      z-index -1
    }
  }

  .header-fix-height {
    height $headerHeight
  }
</style>
