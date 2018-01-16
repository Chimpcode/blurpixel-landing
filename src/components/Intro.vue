<template>
    <div id="front-page">
      <a href="https://github.com/you">
        <img style="position: absolute; top: 0; right: 0; border: 0;"
             src="https://camo.githubusercontent.com/52760788cde945287fbb584134c4cbc2bc36f904/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f6769746875622f726962626f6e732f666f726b6d655f72696768745f77686974655f6666666666662e706e67"
             alt="Fork me on GitHub"
             data-canonical-src="https://s3.amazonaws.com/github/ribbons/forkme_right_white_ffffff.png"></a>
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
export default {
  name: 'intro',
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
.subtitle
  font-size 22px
.github-badgets
  text-align center
</style>
