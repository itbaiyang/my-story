<template>
  <div class="hello">
    <header>
      <div class="header clear">
        <div class="header-left fl">
          <span></span>我们的故事
        </div>
        <div class="header-right fr">
          <div>
            <input type="text"><a>搜索</a>
          </div>
          <a><router-link to="/login">登录</router-link></a>
          <a><router-link to="/register">注册</router-link></a>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>

.header
  width 100%
  height 60px
  padding 5px 15px
  background #34495e
  box-sizing border-box
  font-size 24px
  color #fff
  .header-left
    span
      display inline-block
      width 50px
      height 50px
      background url('../../assets/logo.png') no-repeat center
      background-size 100%
      vertical-align middle
      margin-right 15px
  .header-right
    line-height: 50px
    font-size 18px
    a
      color #fff
      cursor pointer
      margin-right 10px
      vertical-align middle
    a:hover
      color #2196f3
    div
      display inline-block
      vertical-align middle
      line-height 30px
      margin-right 40px
      background #fff
      input
        vertical-align middle
        border none
        outline none
        height 20px
        padding 10px
      a
        vertical-align top
        color #000
        font-size 16px
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
// a {
//   color: #42b983;
// }
</style>
