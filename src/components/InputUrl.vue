<template>
    <div id="input-url">
      <input type="text" class="input" v-model="urlTxt">
      <button class="copy-btn">
        <i class="fa fa-files-o custom-size" aria-hidden="true"></i>
      </button>
    </div>
</template>

<script>
export default {
  name: 'input-url',
  props: {
    shortUrl: String
  },
  computed: {
    urlTxt: {
      set: function (value) {
      },
      get: function () {
        return this.shortUrl
      }
    }
  }
}
</script>

<style scoped lang="stylus">
#input-url
  position relative
  padding 14px 0px
#input-url input
  width  96.5%
  height 40px
.input
  height: 40px
  background: transparent
  border: 5px solid #ffffff8c
  color: #ffffff8c
  font-size 22px
  font-family 'Quicksand'
.copy-btn
  margin 14px 0px
  position absolute
  top 0
  right 0
  bottom 0
  width 55px
.custom-size
  font-size: 24px
</style>
