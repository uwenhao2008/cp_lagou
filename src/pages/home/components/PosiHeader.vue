<template>
    <div class="position-header">
        <div class="position-content">
            <div class="position-content-l">
                <div class="job-name">
                    <div class="company">e签宝基础架构部招聘</div>
                    <div class="name">前端开发工程师 </div>
                </div>
                <dd class="job-request">
                    <p>
                        <span class="salary">10K-20K</span>
                        <span>/杭州 /</span>
                        <span>经验3至5年 /</span>
                        <span>本科及以上 /</span>
                        <span>全职</span>
                    </p>
                    <ul class="position-label clearfix">
                        <li class="labels">地图</li>
                        <li class="labels">视频</li>
                        <li class="labels">WEB前端</li>
                    </ul>
                    <p class="publish_time">09:53&nbsp;发布于拉勾网</p>
                </dd>
            </div>
            <div class="position-content-r">
                <div class="position-deal clearfix">
                    <div class="resume-deliver">
                        <a href="#" class="s-send-btn">
                            投个简历
                        </a>
                    </div>
                    <div class="job-collection"><span class="iconfont icon-collect">&#xe6ae;</span>收藏</div>
                </div>
                <ul class="resume-select clearfix">
                    <li class="resume"><span class="iconfont icon-collect">&#xe620;</span>完善在线简历</li>
                    <li class="resume"><span class="iconfont icon-collect">&#xe631;</span>上传简历附件</li>
                </ul>
                <ul class="tool-list clearfix">
                <!--float：right,所以方向都反了-->
                    <li class="tool-list-icon border-left">
                        <i class="iconfont icon-smallApp">
                            <span class="tool-name tool-name-right">微信扫一扫，用小程序打开</span>
                        </i>
                    </li>
                    <li class="tool-list-icon border-left">
                        <i class="iconfont icon-wechat">
                            <span class="tool-name tool-name-middle">分享到微信</span>
                        </i>
                    </li>
                    <li class="tool-list-icon">
                        <i class="iconfont icon-jubao">
                            <span class="tool-name tool-name-left">举报职位</span>
                        </i>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'PosiHeader'
}
</script>

<style scoped lang="stylus">
  .position-header
    width: 100%
    min-width: 1024px
    background: #f2f5f4
    padding: 30px 0 11px
    .position-content
      width: 1024px
      height: 174px
      margin: 0 auto
      position: relative
      //background : #25a4bb
      .position-content-l
        float: left
        max-width: 696px
        //background : #999
        .job-name
          margin: 0 0 15px
          .company
            margin:-2px 0 8px 0
            font-size: .28rem
            color: #555
          .name
            height: .72rem
            line-height: .72rem
            font-size: .72rem
            color: #333
        .job-request
          display: block
          font-size: .36rem
          p
            margin-bottom: 8px
          .salary
            color: #fd5f39
          .position-label
            display: block
            margin: 0
            padding: 0
            .labels
              float: left
              height: .44rem
              line-height: .44rem
              padding: 0 10px
              margin-right: 8px
              background-color: #ffffff
              color: #70797b
              font-size: 12px
              border-radius: 10px
          .publish_time
            padding-top: 10px
            font-size: 14px
            color: #999
            margin-bottom: 8px
      .position-content-r
        position: absolute
        right: 0
        top: 12px
        max-width: 328px
        //background-color: #ccc
        .position-deal
          position: relative
          //height: .9rem // 设置清除浮动，否则父元素高度塌陷
          .resume-deliver
            float: right
            position: relative
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
          .job-collection
            float: right
            display: inline-block
            height: .88rem
            line-height: .88rem
            width: 104px
            text-align: center
            font-size: .28rem
            color: #00b38a
            border:1px solid #00b38a
            border-radius: 3px
            .icon-collect
              margin-right: 3px
        .resume-select
          margin: 16px 0 10px
          li.resume
            display: list-item
            float: right
            line-height: .56rem
            margin-left: .68rem
        .tool-list
          float: right
          .tool-list-icon
            position: relative
            display: list-item
            float: right
            width: 40px
            height: 20px
            text-align: center
            .iconfont
              font-size: 18px
              color: #c6ced0
              cursor: pointer
            .tool-name
              display: none
              position: absolute
              bottom: 36px
              left: 0
              font-size: 14px
              line-heigh: 18px
              color: #555
              border:2px solid #b7b7b7
              background-color: #fff
              padding: 0 2px
              text-align: center
              z-index: 22
            .icon-jubao
              &:before
                content: "\e652"  // 貌似只能使用unicode 16进制的方式，不能使用 &#xe652;，因为&是stylus的关键字
              &:hover
                .tool-name-left   //hover要把元素hover对！！！~~~~~~~~~~
                  display: inline
                  width: 60px
                  margin-left: -10px
            .icon-wechat
              &:before
                content: "\e7e5"
              &:hover
                .tool-name-middle
                  display: inline
                  width: 70px
                  margin-left: -14px
            .icon-smallApp
              &:before
                content: "\e619"
              &:hover
                .tool-name-right
                  display: inline
                  width: 170px
                  margin-left: -70px
</style>
