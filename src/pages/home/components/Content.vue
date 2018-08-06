<template>
  <div class="container clearfix">
    <div class="content_l">
      <dl class="job-detail">
        <dd class="job-advantage">
          <span class="advantage">职位诱惑</span>
          <p>让我们一起,创造一家,伟大的,公司</p>
        </dd>
        <dd class="job-bt">
          <h3 class="description">职位描述</h3>
          <div>
            <p>职位描述</p>
            <p><br></p>
            <p>1、负责金融类web系统、推⼴活动等前端页面的开发和优化；</p>
            <p>2、与设计、产品及后台开发⼈人员沟通，保证产品的质量和开发 进度 ；</p>
            <p>3、 持续的优化相关的产品的质量、性能、⽤户体验；</p>
            <p><br></p>
            <p>任职要求</p>
            <p>1.一年以上实际开发经验。</p>
            <p>2.熟练使用Angrlar、React、Vue中一种或多种框架。</p>
            <p>3.熟悉gulp、webpack等打包工具。</p>
            <p>4.了解MVC框架；</p>
            <p>5.熟悉页面架构和布局，浏览器的兼容性；</p>
            <p>6.学习能力强，能够读懂开源插件源码，并根据业务需求进行修改。</p>
            <p>7.对于算法和数据结构有一定了解。</p>
            <p>8.计算机相关本科毕业生优先。</p>
          </div>
        </dd>
        <dd class="job_address clearfix">
          <h3 class="address">工作地址</h3>
          <div class="work_address">
            <a href="#">杭州</a> -
            <a href="#">西湖区</a> - 西溪星座
            <a href="#" id="mapPreview">查看地图</a>
          </div>
        </dd>
        <dd class="jd_publisher">
          <h3>职位发布者：</h3>
          <div class="com_border"></div>
        </dd>
      </dl>
    </div>
    <div class="content_r"></div>
  </div>
</template>

<script>
export default {
  name: 'HomeContent'
}
</script>

<style lang="stylus" scoped>
  #mapPreview
    float: right
  .container
    width: 1024px
    margin: 0 auto
    height: 1000px
    //background-color: #c9c9c9
    .content_l
      padding-top: 26px
      width: 696px
      background: url('/static/bgpic/gradient.png') repeat-y
      background-position: right
      padding-right: 52px
      .job-detail
        dd
          padding: 15px 0 10px
        .job-advantage
          .advantage
            font-size: 16px
            font-weight: 700
            color: #333333
            &+p
              margin-top: 13px
              color: #333333
        .job-bt
          font-size: 14px
          line-height: 22px
          & div>p
            margin: 1em 0
          .description
            font-size: 16px
            font-weight: 700
            color: #333333
            line-height: 16px
            margin-bottom: 22px
        .job_address
          margin-top: -26px
          padding-top: 25px
          margin-bpttom: 10px
          .address
            font-size: 16px
            font-weight: 700
            color: #333333
            margin: 10px 0
          .work_address a
            color: #00b38a
            cursor: pointer
        .jd_publisher
          margin-top: 38px
          margin-bottom: 40px
          padding: 5px 0 10px
          position: relative
          & h3
            font-size: 16px
            line-height: 22px
            color: #333333
            font-weight: 700
            position: absolute
            top: -24px
            left: 0
          .com_border
            width: 300px
            height: 300px
            background-color: #c9c9c9
</style>
0
