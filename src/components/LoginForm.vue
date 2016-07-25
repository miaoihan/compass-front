<template>
  <div class="container-login">
    <form>
      <div class="form-group">
        <text-input placeholder="手机号码"></text-input>
      </div>
      <div class="form-group">
        <text-input placeholder="密码" type='password'></text-input>
      </div>
      <div class="form-group link">
        <a>注册</a>
        <a>忘记密码？</a>
      </div>

      <submit-button text="登录"></submit-button>
    </form>
  </div>
</template>

<script>
  import TextInput from './TextInput'
  import SubmitButton from './SubmitButton'
  export default{
    components: {TextInput, SubmitButton}
  }
</script>

<style scoped lang="stylus">


  .container-login {
    margin: 0 auto;
    margin-top .5rem;
    width: 2.7rem;
  }

  .form-group {
    margin .2rem 0
  }

  .link {
    font-size 0.15rem
    display flex
    justify-content space-between
    a {
      color #999999
      display block;
      margin 0 0.1rem;
    }
  }

</style>
