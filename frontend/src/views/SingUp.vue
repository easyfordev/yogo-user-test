<template>
  <div class="sign-up">
    <img src="../assets/goback.png" id="goback" @click="goBack"/>
    <br><br>
    <p><img src="../assets/people.png" width="150px"/></p>
    <p><img src="../assets/phrase1.png" width="250px"/></p>
    <p style="margin-bottom: 40px"><img src="../assets/phrase2.png" width="360px"/></p>
    <label>생년월일을 입력하세요<br><br><input type="date" pattern="\d{4}-\d{2}-\d{2}" v-model="birth_dt" style="border: 1px solid"></label>

    <p class="phrase">11번가 회원이신가요?</p>
    <button class="login-11st-button" @click="click11stLoginBtn">11번가 로그인</button>
    <p class="phrase">아직 11번가 회원이 아니신가요?</p>
    <button class="login-11st-button" @click="click11stSignUpBtn">11번가 회원가입</button>
  </div>
</template>

<script>
export default {
  name: 'SignUp',
  components: {

  },
  data: function () {
    return {
      birth_dt: ''
    }
  },
  methods: {
    goBack () {
      this.$router.push({
        name: 'Landing'
      })
    },
    click11stSignUpBtn: function () {
      if (this.birth_dt === '') {
        alert('생년월일을 입력해주세요')
      } else {
        this.$ga.event('Sign Up', '11번가 로그인', this.birth_dt, 1234)

        this.$router.push({
          name: 'Close'
        })
      }
    },
    click11stLoginBtn: function () {
      if (this.birth_dt === '') {
        alert('생년월일을 입력해주세요')
      } else {
        this.$ga.event('Sign Up', '11번가 회원가입', this.birth_dt, 1234)

        this.$router.push({
          name: 'Close'
        })
      }
    }
  }
}
</script>

<style lang="stylus">
.sign-up
  font-family SansSerif
  position: absolute
  overflow: auto
  top: 50px
  width 100%
  height 90%
  left: 0
  text-align center
  background-color #ffffff
  color #000000

.login-11st-button
  width 300px
  height 50px
  color #ffffff
  font-size 20px
  background-color #f43142
  border 0
.phrase
  margin-top 20px
#goback
  position absolute
  z-index 3
  left 2%
  margin-top 13px
  width 60px
</style>
