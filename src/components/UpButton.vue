<template>
  <div class="upButton" @click="scrollToTop()">
    <i class="upButton__arrow"></i>
  </div>
</template>
<script>
export default {
  name: 'UpButton',

  methods: {
    scrollToTop() {
      // For Safari
      document.body.scrollTop = 0;
      // For Chrome, Firefox, IE and Opera
      document.documentElement.scrollTop = 0;
    }
  }
}
</script>
<style lang="scss" scoped>
  .upButton {
    position: fixed;
    bottom: 52px;
    right: 30px;
  
    &__arrow {
      border: solid black;
      border-width: 0 5px 5px 0;
      display: inline-block;
      padding: 10px;
      
      transform: rotate(-135deg);
      -webkit-transform: rotate(-135deg);

      i {
        font-size: 2em;
      }
    }
  }
</style>