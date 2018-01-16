<template>
    <div id="navbar">
      <chimpcode-banner white class="banner"/>
    </div>
</template>

<script>
import ChimpcodeBanner from '@/components/ChimpcodeBanner'

export default {
  name: 'top-bar',
  components: { ChimpcodeBanner }
}
</script>

<style scoped lang="stylus">
#navbar
  z-index 2
  position: absolute
  min-height 60px
  padding 24px 20px
</style>
