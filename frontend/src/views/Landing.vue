<template>
  <div class="landing">
    <landing-contents source="../assets/intro1.png"></landing-contents>
    <yogo-button></yogo-button>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import YogoButton from '@/components/yogo-button.vue'
import LandingContents from '../components/landing-contents'

export default {
  name: 'Landing',
  components: {
    LandingContents,
    YogoButton
    // HelloWorld
  }
}
</script>

<style lang="stylus">
.landing
  position: absolute
  overflow: auto
  top: 50px
  width 100%
  height: 6000px
  left: 0
  text-align center
  background-color #ffffff
  color #000000
</style>
