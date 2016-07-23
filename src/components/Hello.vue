<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>{{aaa}}</p>
    <p>{{test}}</p>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        // note: changing this line won't causes changes
        // with hot-reload because the reloaded component
        // preserves its current state and we are modifying
        // its initial state.
        msg: 'Hello World',
        aaa: 'nihao',
        test: 'aaaa'
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
  $color = #42b983
  h1 {
    color: $color;
  }
</style>
