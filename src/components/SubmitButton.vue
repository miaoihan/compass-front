<template>
  <div class="submit-wrapper">
    <button class="btn-clear submit" @click="click" type="button" :style=" {backgroundColor: backgroundColor}">{{text}}</button>
  </div>
</template>

<script>
  export default{
    data () {
      return {
        msg: 'hello vue'
      }
    },
    props: {
      text: {
        type: String,
        default: '确认'
      },
      backgroundColor: {
        type: String,
        default: '#0e2d60'
      }
    },
    components: {},
    methods: {
      click () {
        console.log(this.backgroundColor)
        return false
      }
    }
  }
</script>

<style scoped lang="stylus">
  .submit-wrapper {
    position relative
  }

  .submit {
    width 100%
    height 0.4rem;
    font-size 0.18rem
    font-weight 700
    display block
  }
</style>
