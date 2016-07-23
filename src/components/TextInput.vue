<template>
  <div class="input-wrapper">
    <input type="{{type}}" placeholder="{{placeholder}}" class="text-input">
  </div>
</template>

<script>
  export default{
    data () {
      return {test: 'nihao'}
    },
    props: {
      type: {type: String, default: 'text'},
      placeholder: {type: String, default: ''},
      value: {
        twoWay: true
      }
    },
    components: {},
    methods: {
      notify () {
      }
    }
  }
</script>

<style scoped lang="stylus">
  .input-wrapper {
    position relative
  }

  .text-input {
    display block
    height 0.4rem
    width 100%
    border none
    font-size 0.17rem
    padding-left 0.2rem
    padding-right 0.2rem
    &:active, &:focus {
      border none
      outline: none;
    }
  }
</style>
