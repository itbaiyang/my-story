<template>
  <div class="home">
    <header>
      <div class="header clear">
        <div class="header-left fl">
          <span></span>我们的博客
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
    <div class="container">
      <div class="fl">
        <article>
          <div class="article">
            <carrousel class="swiper"></carrousel>
            <div class="tags">
              <div class="tag"><img src="@/assets/logo.png"><span>摄影协会</span></div>
              <div class="tag"><img src="@/assets/logo.png"><span>摄影协会</span></div>
              <div class="tag"><img src="@/assets/logo.png"><span>摄影协会</span></div>
              <div class="tag"><img src="@/assets/logo.png"><span>摄影协会</span></div>
              <div class="tag"><img src="@/assets/logo.png"><span>摄影协会</span></div>
              <div class="tag"><img src="@/assets/logo.png"><span>摄影协会</span></div>
              <div class="tag"><img src="@/assets/logo.png"><span>摄影协会</span></div>
              <div class="tag"><img src="@/assets/logo.png"><span>摄影协会</span></div>
              <div class="tag"><img src="@/assets/logo.png"><span>摄影协会</span></div>
            </div>
            <hr />
            <section>
              <div class="blog">
                <!-- <h1>blog-list</h1> -->
                <ul>
                  <li>
                    <p class="title">我的博客</p>
                    <div class="content">
                      这是我的有一个好的博客文章
                    </div>
                  </li>
                  <li>
                    <p class="title">我的博客</p>
                    <div class="content">
                      这是我的有一个好的博客文章
                    </div>
                  </li>
                  <li>
                    <p class="title">我的博客</p>
                    <div class="content">
                      这是我的有一个好的博客文章
                    </div>
                  </li>
                  <li>
                    <p class="title">我的博客</p>
                    <div class="content">
                      这是我的有一个好的博客文章
                    </div>
                  </li>
                  <li>
                    <p class="title">我的博客</p>
                    <div class="content">
                      这是我的有一个好的博客文章
                    </div>
                  </li>
                </ul>
              </div>
            </section>
          </div>
        </article>
      </div>
      <div class="fr">
        <aside>
          <div class="aside">
            <div class="theme">
              <a>a</a>
              <a>a</a>
              <a>a</a>
              <a>a</a>
              <a>a</a>
            </div>
            <div class="ad">
              <!-- <img src="@/assets/logo.png"> -->
            </div>
            <div class="author">
              <p class="title">title</p>
              <ul>
                <li>
                  <div>
                    <p>白杨</p>
                    <p>2018.06.08</p>
                  </div>
                </li>
                <li>a</li>
                <li>z</li>
              </ul>
            </div>
          </div>
        </aside>
      </div>
    </div>
  </div>
</template>

<script>
import 'swiper/dist/css/swiper.css'

import carrousel from './Swiper.vue'

export default {
  name: 'HelloWorld',
  components: {
    carrousel
  },
  data () {
    return {
      src: '@/assets/logo.png'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.home
  height 100%
  padding-top 60px
  overflow auto
  .header
    position fixed
    top 0
    z-index 999
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
        vertical-align top
      a:hover
        color #2196f3
      div
        display inline-block
        vertical-align middle
        line-height 30px
        margin-right 40px
        background #fff
        border-radius 4px
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
  .container
    width 960px
    overflow hidden
    margin 15px auto
    .article
      .swiper
        border-radius 6px
      .tags
        width 635px
        margin-top 20px
        margin-left -10px
        margin-bottom 20px
        line-height 46px
        .tag
          margin-left 10px
          height 34px
          line-height 34px
          display inline-block
          background #e0e0e0
          padding-right 10px
          border-radius 4px
          img
            width 34px
            height 34px
            vertical-align top
            border-radius 4px
          span
            padding-left 10px
      .blog
        ul
          li
            box-sizing border-box
            border-bottom 1px solid #cacaca
            height 140px
            margin: 10px 0
            padding 10px 0
            .title
              font-size .4rem
              font-weight 700
            .content
              font-size .28rem
              color #888888
    .aside
      width 300px
      .theme
        width 100%
        a
          display block
          background #e0e0e0
          line-height 36px
          font-size .28rem
          margin-bottom 6px
          border-radius 4px
          padding 7px 15px
      .ad
        margin-top 20px
        width 300px
        height 200px
        border 1px solid #e0e0e0
        background $themeBlue
        img
          width 100%
          height 100%
      .author
        margin-top 10px
        .title
          line-height 36px
        ul
          li
            padding 0 15px
            background #e0e0e0
            line-height 50px
            font-size .28rem
            margin-bottom 10px
            border-radius 4px
            div
              p
                line-height 20px
</style>
