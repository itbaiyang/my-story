<template>
  <div class="login">
    <div class="login-title">
      <p>业精于勤而荒于嬉</p>
      <p style="text-align:center">行成于思而毁于随</p>
    </div>
    <div class="login-box">
      <h1>加入我们吧</h1>
      <form>
        <div class="form-item">
          <label for="account">账号</label>
          <input type="text" name="account">
        </div>
        <div class="form-item">
          <label for="password">密码</label>
          <input type="text" name="password">
        </div>
        <div class="form-item">
          <button>登录</button>
        </div>
      </form>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Login',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>
<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.login
  width 100%
  height 100%
  display flex
  // flex-direction column
  justify-content center
  align-items center
  background #fff
  .login-title
    width 500px
    p
      font-size 28px
      line-height 60px
      letter-spacing 6px
  .login-box
    width 420px
    height 380px
    background #f2f2f2
    border-radius 4px
    box-shadow 2px 2px 1px 1px #e0e0e0
    padding 30px 15px
    h1
      font-size .4rem
      letter-spacing 2px
      color $themeRed
      text-align center
      font-weight 600
      padding 20px 0
    label
      width 60px
      letter-spacing 4px
      line-height 36px
      font-size .36rem
    .form-item
      box-sizing border-box
      padding 12px 20px
      height 60px
      line-height 36px
      input
        width 300px
        height 36px
        vertical-align top
      button
        width 300px
        margin-left 49px
        background $themeGreen
        color #fff
        line-height 36px
        height 36px
        border-radius 4px
</style>
