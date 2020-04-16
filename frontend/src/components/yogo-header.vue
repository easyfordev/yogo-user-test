<template>
  <div class="yogo-header">
    <img src="../assets/YOGO_logo.png" id="logo" @click="goHome">
      <!-- <span>hi</span>
      <img alt="logo" src="../assets/11STREET_black.png"> -->
  </div>
</template>

<script>
export default {
  name: 'YogoHeader',
  methods: {
    goHome () {
      this.$router.push({
        name: 'Landing'
      })
    }
  }
}
</script>

<style scoped lang="stylus">
.yogo-header
  position: fixed
  z-index 10
  top 0
  width: 100%
  height: 50px
  left: 0
  background-color: #ffffff
  border-top: 2px solid #f43142
  border-bottom: 2px solid #f43142
#logo
  width 90px
  margin-top 15px
</style>
