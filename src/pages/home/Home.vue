<template>
  <div>
    <home-header></home-header>
    <home-posi-header></home-posi-header>
    <common-fade></common-fade>
    <keep-alive>
      <home-banner></home-banner>
    </keep-alive>
    <div class="homebody">
      <p style="font-size: 28px">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam consequuntur, delectus illum laudantium minima perferendis quam rep Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab hic nulla perferendis quidem voluptatem. A doloribus earum exercitationem, iure nostrum pariatur qui saepe. Enim iusto, placeat. Aperiam consectetur culpa quae?udiandae s Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad autem consequuntur cum dolorem error exercitationem harum nam, natus non odit officia ratione, rerum sint tempora veniam? Commodi fuga nisi ratione!oluta tempo Lorem ipsum dolor sit amet, consectetur adipisicing elit. Autem cupiditate eos quam sit? Accusamus culpa dolor harum ipsam maxime molestias nam necessitatibus, perferendis qui repellat sint suscipit tempore unde voluptatibus!ra voluptat Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus amet architecto aut blanditiis cum cupiditate deserunt ducimus, eaque inventore iste magni molestiae, mollitia nisi praesentium quaerat repellendus similique sunt voluptates.e? Ea ex ex Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae blanditiis commodi dolor excepturi fugit optio quas. Assumenda blanditiis cupiditate exercitationem facilis, illum libero modi perspiciatis porro possimus quasi quibusdam quisquam?plicabo facilis ipsa libero nisi odit quo, quod. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto dignissimos nam provident repellendus sunt ullam voluptatem? Aliquid architecto atque commodi culpa, excepturi impedit provident quidem reiciendis sed sit soluta, ullam!</p>
    </div>
  </div>
</template>

<script>
import HomeHeader from '@/pages/home/components/Header'
import HomePosiHeader from '@/pages/home/components/PosiHeader'
import CommonFade from '@/common/fade/FadeAnimation'
import HomeBanner from '@/pages/home/components/Banner'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomePosiHeader,
    CommonFade,
    HomeBanner
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="stylus" scoped>
  .homebody
    height: 1000px
</style>
