<template>
  <div id="cc-section" class="blrpxl-txt-font" :style="{ 'background': bckgrnd, 'color': textColor}">
    <slot>Hello There</slot>
  </div>
</template>

<script>
export default {
  name: 'CcSection',
  props: {
    bckgrnd: String,
    textColor: String
  }
}
</script>

<style lang="stylus">
#cc-section
  min-height 200px
  background-color #efffff
  padding 4em 5em
.one-column
  width 100%
  text-align center
.two-column
  width 100%
  text-align center
</style>
