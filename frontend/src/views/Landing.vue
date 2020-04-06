<template>
  <div class="landing">
    <h1>Contents</h1>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Landing',
  components: {
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
  height: 2000px
  left: 0
  text-align center
  background-color #ffffff
  color #000000
</style>
