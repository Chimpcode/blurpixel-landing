<template>
    <div id="home">
      <topbar></topbar>
      <cc-intro height-size="100vh"></cc-intro>
      <cc-section>
        <div class="hm-container">
          <div class="hm-title cc-h1">Hello there</div>
        </div>
      </cc-section>
      <cc-section bckgrnd="#000" text-color="#fff">
        <div class="hm-container">
          <div class="hm-title cc-h2">Look at this pics</div>
        </div>
        <div class="hm-grid">
          <template v-for="(item, i) in showcaseImgs">
            <div :key="i" class="img-item">
              <img :src="item" alt=""
                   width="300" height="300"
                   >
              <input-url :short-url="item"></input-url>
            </div>
          </template>
        </div>
      </cc-section>
      <cc-section>
        <div class="hm-container">
          <div class="hm-title">Hello there</div>
        </div>
      </cc-section>
      <cc-footer></cc-footer>
    </div>
</template>

<script>
import CcIntro from '@/components/CCIntro'
import CcSection from '@/components/CCSection'
import CcFooter from '@/components/CCFooter'
import Topbar from '@/components/Topbar'
import InputUrl from '@/components/InputUrl'

export default {
  components: { CcIntro, CcSection, CcFooter, Topbar, InputUrl },
  name: 'home',
  data () {
    return {
      showcaseImgs: [
        'https://source.unsplash.com/random/300x300',
        'https://source.unsplash.com/random/300x300',
        'https://source.unsplash.com/random/300x300',
        'https://source.unsplash.com/random/300x300',
        'https://source.unsplash.com/random/300x300'
      ]
    }
  }
}
</script>

<style scoped lang="stylus">
.hm-title
  text-align center
@media screen and (min-width: 601px)
  .hm-title
    height 200px
    line-height 200px
@media screen and (max-width: 600px)
  .hm-title
    font-size 32px
    margin-top 50px
.align-to-left
  text-align left
.align-to-right
  text-align right
.align-to-center
  text-align center
.hm-container
  position relative
.hm-grid
  display flex
  flex-direction row
  flex-wrap wrap
  justify-content center
  align-content stretch
.img-item
  flex-basis auto
  padding 10px
  margin 10px
</style>
