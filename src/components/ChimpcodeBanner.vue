<template>
    <div id="banner">
      <!--<span class="logo">Chimpcode</span>-->
      <a href="">
        <img v-if="white" :class="{ 'white': white, 'logo-img': true }" src="../assets/chimpbannerleftwhite.svg"
             alt="">
        <img v-else :class="{ 'white': white, 'logo-img': true }" src="../assets/chimpbannerleft.svg"
             alt="">
      </a>
    </div>
</template>

<script>
export default {
  name: 'chimpcode-banner',
  props: {
    white: {
      type: Boolean,
      default: false
    }
  },
  mounted () {
  }
}
</script>

<style scoped lang="stylus">
#banner
  display inline-block
  font-family 'Quicksand', sans-serif
#banner > .logo
  font-size 28px

@media screen and (max-width: 600px)
  #banner > .logo
    font-size 22px

.white
  color: #fff
.logo-img
  width: 150px
</style>
