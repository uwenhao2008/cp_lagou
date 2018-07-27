<template>
  <div id="header">
    <!--顶部黑色导航-->
    <div id="lg_tbar">
      <div class="inner">
        <div class="lg_bar_1">
          <a href="#" class="lg_app">拉勾APP</a>
          <a href="#" class="log_os">进入企业版</a>
        </div>
        <ul class="lg_bar_r">
          <li><a href="#">消息</a></li>
          <li><a href="#">我的简历</a></li>
          <li><a href="#">投递箱</a></li>
          <li><a href="#">收藏夹</a></li>
          <li><a href="#">用户名</a></li>
        </ul>
      </div>
    </div>
    <!--底部白色导航-->
    <div id="lg_tnav">
      <div class="inner">
        <div class="lg_tnav_1">
          <a href="#"><h1>拉勾网</h1></a>
        </div>
        <ul class="lg_tnav_wrap">
          <li><a href="#">首页</a></li>
          <li><a href="#">公司</a></li>
          <li><a href="#">校园</a></li>
          <li><a href="#">言职</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
  #header
    min-width : 1024px
    #lg_tbar
      height: .6rem
      font-size: .28rem
      background: #333
      .inner
        position: relative
        //max-width : 1308px
        width: 1200px
        margin : 0 auto
        padding: 0 60px
        .lg_bar_1
          float: left
          line-height: .6rem
          a.lg_app
            color: #08d7a2
            padding: 0 .24rem 0 .54rem
            //background url('/static/icons/app_icon_0495d1d.png') 10px 0 no-repeat
            //background: url('~@/assets/icons/app_icon_0495d1d.png') 10px 0 no-repeat
            // 这里不要background-image了，因为那个只是添加图片，没有别的属性方式的
            background: url(//www.lgstatic.com/www/static/common/widgets/header_c/modules/img/app_icon_0495d1d.png) 10px 0 no-repeat
          a.log_os
            line-height: .3rem
            border-left: 1px solid #5d5d5d
            padding:0 .24rem
            color: #c4c3c3
            &:hover
              color:  #fff   //伪类选择没起作用，why？  只有一个冒号~~！！
    .lg_bar_r
      float: right
      li
        float: left
        line-height: .3rem
        border-left: 1px solid #5d5d5d
        padding:0 .24rem
        margin:.14rem 0 0
        a
          color: #c4c3c3
          &:hover
            color:  #fff   //伪类选择没起作用，why？  只有一个冒号~~！！
    #lg_tnav
      height: 1.08rem
      border-top: 1px solid #d2d2d2
      border-bottom: 1px solid #e5e5e5
      background-color: #fafafa
      .inner
        width: 1024px
        margin:0 auto
        .lg_tnav_1
          width: 5.2rem
          float: left
          a h1
            float: left
            width: 97px
            height: 34px
            margin:10px 0 0
            padding:0
            background-image: url(//www.lgstatic.com/www/static/common/widgets/header_c/modules/img/logo_1c5763c.png)
            text-indent : -99em  // 文本缩进，变相隐藏了h1标签  其实h1的作用就是给a标签提供背景图而已
        .lg_tnav_wrap
          float: left
          li
            display: inline-block
            //box-sizing: border-box
            margin: 0 .32rem
            position: relative
            &:hover
              color: #333
              border-bottom:2px solid #00b38a
            a
              //display: block
              font-size : .36rem
              line-height: 1.06rem
              padding: 0 .1rem
              color: #999
</style>
