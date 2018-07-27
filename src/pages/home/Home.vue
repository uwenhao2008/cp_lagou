<template>
  <div>
    <home-header></home-header>
    <home-posi-header></home-posi-header>
  </div>
</template>

<script>
import HomeHeader from '@/pages/home/components/Header'
import HomePosiHeader from '@/pages/home/components/PosiHeader'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomePosiHeader
  }
}
</script>

<style lang="stylus" scoped>

</style>
