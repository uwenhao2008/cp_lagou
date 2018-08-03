<template>
  <div :class="[!isShow?'':'ceil-transition','ceil']" v-show="isShow" ref="headerFix">
    <div class="ceil-content">
      <span class="ceil-job">前端大师 /</span>
      <span class="ceil-salary">5K-10K</span>
      <div class="ceil-right">
        <div class="resume-deliver">
          <a href="#" class="s-send-btn">
            投个简历
          </a></div>
        <div class="job-collection"><span class="iconfont icon-collect">&#xe6ae;</span>收藏</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeBanner',
  data () {
    return {
      isShow: false
    }
  },
  activated () {
    window.addEventListener('scroll', this.handleScroll)
  },
  deactivated () {
    window.removeEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll () {
      // console.log('监听滚动事件')
      const top = document.documentElement.scrollTop
      if (top > 230) {
        // console.log(this.$refs.headerFix)
        console.log(top)// 这里实现height动态变化  到70以后  在设置isShow为true
        this.isShow = true
      } else {
        this.isShow = false
      }
    }
  }
}
</script>

<style lang="stylus" scoped>
  .ceil-transition
    position: fixed    // 这里没有执行？why
    z-index: 1000
    top: 0
    left: 0
    right: 0
    background-color: rgba(242,245,244,.9)
    height: 0
    transition: height 0.5s linear
    height: 70px
  .ceil
    position: fixed
    z-index: 1001
    top: 0
    left: 0
    right: 0
    height: 70px
    background-color: rgba(242,245,244,.9)
    overflow: hidden
    .ceil-content
      width: 1024px
      height: 70px
      margin: 0 auto
      line-height: 70px
      font-size: 18px
      .ceil-job
        color: #333333
        font-weight: 700
      .ceil-salary
        color: #fd5f39
        font-weight: 700
      .ceil-right
        float: right
        display: inline-block
        height: 70px
        padding: 12px 0
        .resume-deliver
          float: right
          position: relative
          height: 44px
          line-height: 44px
          .s-send-btn
            display: inline-block //不设置这个，背景色是撑不满设定的height的
            height: .88rem
            line-height: .88rem
            font-size: .36rem
            color: #fff
            background: #00b38a
            border: 1px solid #00b38a
            margin-left: 17px
            padding: 0 33px
            border-radius: 3px
            &:hover
              background: #00a57f
        .job-collection
          float: right
          display: inline-block
          height: 44px
          line-height: 44px
          width: 104px
          text-align: center
          font-size: .28rem
          color: #00b38a
          border:1px solid #00b38a
          border-radius: 3px
          &:hover
            color: #00a57f
          .icon-collect
            margin-right: 3px
</style>
