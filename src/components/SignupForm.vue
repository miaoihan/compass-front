<template>
  <div class="container-signup">
    <form>
      <div class="form-group">
        <text-input placeholder="手机号码"></text-input>
      </div>
      <div class="form-group">
        <text-input placeholder="密码"></text-input>
      </div>
      <div class="form-group">
        <captcha-input placeholder="验证码"></captcha-input>
      </div>
      <div class="form-group">
        <sms-captcha-input placeholder="短信验证码"></sms-captcha-input>
      </div>

      <div class="form-group link">
        注册即同意<a>《指南针用户协议》</a>

      </div>


      <submit-button text="注册"></submit-button>

    </form>
  </div>

</template>

<script>
  import TextInput from './TextInput'
  import SubmitButton from './SubmitButton'
  import CaptchaInput from './CaptchaInput'
  import SmsCaptchaInput from './SmsCaptchaInput'
  export default{
    components: {SubmitButton, TextInput, CaptchaInput, SmsCaptchaInput}
  }
</script>

<style scoped lang="stylus">
  .container-signup {
    margin: 0 auto;
    margin-top .5rem;
    width: 2.7rem;
  }

  .form-group {
    margin .2rem 0
  }

  .link {
    font-size 0.15rem
    color #999999
    a {
      text-decoration: underline
    }
  }

</style>
