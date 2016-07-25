<template>
  <compass-header :need-fix-height="false"></compass-header>
  <evaluate-nav></evaluate-nav>
  <evaluate-item></evaluate-item>
  <evaluate-item></evaluate-item>
</template>

<script>
  import CompassHeader from '../components/CompassHeader'
  import EvaluateNav from '../components/EvaluateNav'
  import EvaluateItem from '../components/EvaluateItem'

  export default{
    components: {CompassHeader, EvaluateNav, EvaluateItem}
  }
</script>

<style scoped lang="stylus">


</style>
