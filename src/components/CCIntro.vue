<template>
    <div id="front-page">
      <github-corner link="https://github.com/Chimpcode/blurpixel"/>
      <div class="title-container blrpxl-font">
        <div class="title cc-h0">{{title}}</div>
        <p class="subtitle">{{subtitle}}</p>
        <!-- Place this tag where you want the button to render. -->
        <div class="github-badgets">
          <a class="github-button"
             href="https://github.com/Chimpcode/blurpixel"
             data-icon="octicon-star" data-size="large"
             data-show-count="true" aria-label="Star Chimpcode/blurpixel on GitHub">Star</a>
          <!-- Place this tag where you want the button to render. -->
          <a class="github-button"
             href="https://github.com/Chimpcode"
             data-size="large"
             data-show-count="true"
             aria-label="Follow @Chimpcode on GitHub">Follow @Chimpcode</a>
        </div>
      </div>
    </div>
</template>

<script>
import GithubCorner from '@/components/GithubCorner'
export default {
  name: 'intro',
  components: {
    GithubCorner
  },
  data () {
    return {
      title: 'Blur Pixel',
      subtitle: 'Lorem ipsum asdsadasdsa asdsadasdsa asdasdsadas dsadasdasa'
    }
  }
}
</script>

<style scoped lang="stylus">

.cc-h0
  font-size 92px
  /*url("https://images.unsplash.com/photo-1444090695923-48e08781a76a?auto=format&fit=crop&w=1950&q=80") center center no-repeat*/
#front-page
  background: url('https://images.unsplash.com/photo-1444090695923-48e08781a76a?auto=format&fit=crop&w=1950&q=80'),
    linear-gradient(#377b80 0%, #882d4f 90%)
  background-blend-mode: overlay;
  width 100%
  height 100vh
  position relative
#front-page:before
  opacity 0.4
.title-container
  position absolute
  left 50%
  transform translateY(-50%) translateX(-50%)
  top: 50%;
  color: white
.title
  text-align center
  text-shadow: 0 0 5px #fff, 0 0 10px #fff, 0 0 20px #7D95B1, 0 0 30px #7D95B1, 0 0 40px #7D95B1, 0 0 55px #7D95B1, 0 0 75px #7D95B1;
.subtitle
  font-size 22px
.github-badgets
  text-align center

</style>
