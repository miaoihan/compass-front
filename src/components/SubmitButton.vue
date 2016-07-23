<template>
  <div class="submit-wrapper">
    <button class="btn-clear submit">{{text}}</button>
  </div>
</template>

<script>
  export default{
    data () {
      return {
        msg: 'hello vue',
        style: {}
      }
    },
    props: {
      text: {
        type: String,
        default: '确认'
      },
      color: {
        type: String,
        default: '#0e2d60'
      }
    },
    components: {},
    methods: {}
  }
</script>

<style scoped lang="stylus">
  .submit-wrapper {
    position relative
  }

  .submit {
    width 2.7rem;
    height 0.4rem;
    font-size 0.18rem
  }
</style>
