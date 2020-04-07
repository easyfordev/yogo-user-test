<template>
  <div class="sign-up">
    <img src="../assets/goback.png" id="goback" @click="goBack"/>

    <h3 id="anouncement"> <img src="../assets/YOGO_logo.png" width="50px"/>하기 위해서는 11번가 계정이 필요합니다.</h3>

    <label>생년월일을 입력하세요 : <input type="date"/></label>
    <p class="question">11번가 회원이신가요?</p>
    <button class="login-11st-button" @click="goClose">11번가 로그인</button>
    <p class="question">아직 11번가 회원이 아니신가요?</p>
    <button class="login-11st-button" @click="goClose">11번가 회원가입</button>
  </div>
</template>

<script>
export default {
  name: 'SignUp',
  components: {

  },
  methods: {
    goBack () {
      this.$router.push({
        name: 'Landing'
      })
    },
    goClose () {
      this.$router.push({
        name: 'Close'
      })
    }
  }
}
</script>

<style lang="stylus">
.sign-up
  position: absolute
  overflow: auto
  top: 50px
  width 100%
  height 100%
  left: 0
  text-align center
  background-color #ffffff
  color #000000

#anouncement
  margin-top 100px
  margin-bottom 50px
.question
  margin-top 50px
  margin-bottom 20px

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
