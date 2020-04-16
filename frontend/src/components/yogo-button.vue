<template>
  <div class="yogo-button">
    <button id="goyogo" @click="clickBtn">YOGO 시작하기</button>
  </div>
</template>

<script>
export default {
  name: 'YogoButton',
  methods: {
    clickBtn: function () {
      this.$ga.event('Button click', 'YOGO 하기', 'YOGO하기', 1234)

      this.$router.push({
        name: 'SingUp'
      })
    }
  }
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
  height: 70px
#label
  color #000000
#goyogo
  position absolute
  left 0
  top 0
  width 100%
  height 100%
  font-size 20px
  color #ffffff
  background-color #f43142
</style>
