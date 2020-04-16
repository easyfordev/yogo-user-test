<template>
  <div class="close">
    <img src="../assets/goback.png" id="goback" @click="goBack"/>
    <br><br>
    <!--<h3 id="anouncement">감사합니다</h3>-->
    <!--<p class="question">-->
      <!--이 설문은 11번가의 신규 서비스 런칭과 관련하여<br>사전 조사를 위해 가상으로 구현된 페이지입니다.<br><br>-->
      <!--실제 11번가 회원가입은 이루어지지 않으며,<br> 개인정보도 연동 되지 않습니다.<br><br>-->
      <!--설문에 참여해주셔서 진심으로 감사합니다.<br>-->
    <!--</p>-->
    <p style="margin-top: 100px"><img src="../assets/phrase3.png" width="130px"/></p>
    <p style="margin-top: 80px"><img src="../assets/phrase4.png" width="360px"/></p>
  </div>
</template>

<script>
export default {
  name: 'Close',
  methods: {
    goBack () {
      this.$router.push({
        name: 'SingUp'
      })
    }
  }
}
</script>

<style lang="stylus">
.close
  position: absolute
  overflow: auto
  top: 50px
  width 100%
  height 90%
  left: 0
  text-align center
  background-color #ffffff
  color #000000

#anouncement
  margin-top 100px
  margin-bottom 50px

.question
  margin-top 100px
  margin-bottom 20px
  margin-left 5%
  margin-right 5%

.login-11st-button
  width 300px
  height 50px
  color #ffffff
  font-size 20px
  background-color #f43142
  border 0

#goback
  position absolute
  z-index 3
  left 2%
  margin-top 13px
  width 60px
</style>
