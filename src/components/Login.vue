<template>
  <form>
    <text-input placeholder="手机号码"></text-input>
    <text-input placeholder="密码"></text-input>
    <submit-button text="登录"></submit-button>
  </form>
</template>

<script>
  import TextInput from './TextInput'
  import SubmitButton from './SubmitButton'
  export default{
    components: {TextInput, SubmitButton}
  }
</script>

<style scoped lang="stylus">

  .submit {
    background-color #0e2d60
    font-size 0.2rem;
    color #fff;

  }

</style>
