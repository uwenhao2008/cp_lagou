<template>
  <div>
    <home-header></home-header>
    <home-posi-header></home-posi-header>
    <common-fade></common-fade>
    <keep-alive>
      <home-banner></home-banner>
    </keep-alive>
    <home-content></home-content>
  </div>
</template>

<script>
import HomeHeader from '@/pages/home/components/Header'
import HomePosiHeader from '@/pages/home/components/PosiHeader'
import CommonFade from '@/common/fade/FadeAnimation'
import HomeBanner from '@/pages/home/components/Banner'
import HomeContent from '@/pages/home/components/Content'

export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomePosiHeader,
    CommonFade,
    HomeBanner,
    HomeContent
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="stylus" scoped>
</style>
