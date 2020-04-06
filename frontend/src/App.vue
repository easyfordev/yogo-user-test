<template>
  <div id="app">
    <!-- 1. Header  -->
    <yogo-header></yogo-header>
    <!-- 2. Contents  -->
    <landing></landing>
    <!-- 3. Footer  -->
    <yogo-button></yogo-button>

    <router-view/>
  </div>
</template>

<script>
// @ is an alias to /src
import YogoHeader from '@/components/yogo-header.vue'
import Landing from '@/views/Landing.vue'
import YogoButton from '@/components/yogo-button.vue'

export default {
  components: {
    YogoHeader,
    Landing,
    YogoButton
  }
}
</script>

<style lang="stylus">
#app
  // font-family Avenir, Helvetica, Arial, sans-serif
  // -webkit-font-smoothing antialiased
  // -moz-osx-font-smoothing grayscale
  text-align center
  // color #2c3e50
  background-color red
</style>
