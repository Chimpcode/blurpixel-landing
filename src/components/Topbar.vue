<template>
  <div id="navbar">
    <chimpcode-banner white class="banner"/>
    <div class="links">
      <a :key="i" v-for="(item, i) in links" :href="item.url" class="link">{{item.name}}</a>
    </div>
  </div>
</template>

<script>
import ChimpcodeBanner from '@/components/ChimpcodeBanner'

export default {
  name: 'top-bar',
  components: { ChimpcodeBanner },
  props: {
    links: { type: Array, default: () => { return [] } }
  }
}
</script>

<style scoped lang="stylus">
  #navbar
    z-index 2
    position: absolute
    min-height 60px
    padding 24px 20px
  .banner
    position relative
    top 12px
  .links
    display inline-block
    margin-left 50px
  .link
    text-decoration none
    color white
    font-size 16px
    margin 8px 10px
    padding 8px 10px
</style>
