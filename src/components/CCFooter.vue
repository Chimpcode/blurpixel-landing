<template>
    <div id="cc-footer">
      <div id="footer-content">
        <div class="section-container blurpixel-side">
          <span class="blrpxl-title">Blur Pixel</span>
        </div>
        <div class="section-container links-side">
          <div class="links">
            <p><a href="">Documentacion</a></p>
            <p><a href="">About Us</a></p>
            <p><a href="">Buy me a coffee</a></p>
          </div>
        </div>
        <div class="section-container chimpcode-side">
          <chimpcode-banner white></chimpcode-banner>
          <p>
            <a href="">
              <i class="fa fa-2x fa-facebook-square" aria-hidden="true"></i>
            </a>
            <a href="">
              <i class="fa fa-2x fa-github-alt" aria-hidden="true"></i>
            </a>
            <a href="">
              <i class="fa fa-2x fa-twitter-square" aria-hidden="true"></i>
            </a>
          </p>
        </div>
      </div>
    </div>
</template>

<script>
import ChimpcodeBanner from '@/components/ChimpcodeBanner'
export default {
  name: 'cc-footer',
  components: {
    ChimpcodeBanner
  }
}
</script>

<style lang="stylus" scoped>
#cc-footer
  min-height 250px
  background-color #2d2e3b

#footer-content
  width 100%
  display flex
  flex-direction row
  flex-wrap wrap
  justify-content space-evenly
  align-content stretch

@media screen and (min-width: 1744px)
  #footer-content
    max-width 80%
    left 50%
    position relative
    transform translateX(-50%)

#cc-footer > div
  flex-grow 1
  flex-basis auto
.chimpcode-side
  text-align right
  padding-right 3.0em
.chimpcode-side p
  margin-top 32px
.chimpcode-side a
  text-decoration none
  margin 1px 8px
.chimpcode-side i
  color white

.links-side
  text-align center
  padding-left 2em
  padding-right 2em

.links-side a
  color white
  font-family 'Quicksand', sans-serif
  text-decoration none
.links
  position relative;
  top 50%;
  transform translateY(-80%) translateX(-50%)
  left 50%

.blurpixel-side
  text-align left
  padding-left 3.0em
.blrpxl-title
  color white
  font-family 'Megrim', cursive
  font-weight bold
  font-size 28px
.section-container
  margin 3em 30px 18px 30px

/*744*/
@media screen and (max-width: 744px)
  .links-side
    text-align center
    width 100%
  .chimpcode-side
    text-align center
    padding-right 0em
  .blurpixel-side
    text-align center
    padding-left 0em

</style>
