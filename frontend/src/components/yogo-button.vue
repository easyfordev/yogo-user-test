<template>
  <div class="yogo-button">
    <h3 id="label">YOGO 시작하기</h3>
  </div>
</template>

<script>
export default {
  name: 'YogoButton'
}
</script>

<style scoped lang="stylus">
.yogo-button
  position: fixed
  text-align center
  z-index 3
  bottom 0
  left 0
  width: 100%
  height: 50px
  background-color: #F13447
#label
  color #000000
</style>
