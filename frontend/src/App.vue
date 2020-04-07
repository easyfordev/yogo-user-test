<template>
  <div id="app">
    <yogo-header></yogo-header>
    <router-view/>
  </div>
</template>

<script>
// @ is an alias to /src
import YogoHeader from '@/components/yogo-header.vue'

export default {
  components: {
    YogoHeader
  }
}
</script>

<style lang="stylus">
@import url('https://fonts.googleapis.com/css?family=Noto+Sans+KR&display=swap');

#app
  // font-family Avenir, Helvetica, Arial, sans-serif
  // -webkit-font-smoothing antialiased
  // -moz-osx-font-smoothing grayscale
  text-align center
  // color #2c3e50
  background-color red

</style>
