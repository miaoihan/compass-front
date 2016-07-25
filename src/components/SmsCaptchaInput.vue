<template>
  <div class="input-wrapper">
    <input type="{{type}}" placeholder="{{placeholder}}" class="text-input">
    <a class="sms-get">获取验证码</a>
  </div>
</template>

<script>
  export default{
    components: {},
    props: {
      type: {type: String, default: 'text'},
      placeholder: {type: String, default: ''},
      value: {
        twoWay: true
      }
    }
  }
</script>

<style scoped lang="stylus">
  .input-wrapper {
    position relative
    width 100%
    height 0.4rem
    background #fff
    display flex
    align-items center
    justify-content space-between
  }

  .text-input {

    display block
    height 0.4rem
    border none
    width 0.8rem;
    max-width 1.4rem;
    font-size 0.17rem
    padding-left 0.2rem
    padding-right 0.2rem
    flex-grow 1

    &:active, &:focus {
      border none
      outline: none;
    }
  }

  .sms-get {
    display block;
    font-size 0.14rem;
    margin 0 .1rem
    color #999999;
  }

</style>
