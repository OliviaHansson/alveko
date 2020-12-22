<template>
  <div id="app">
    <Shell />
  </div>
</template>

<script>
import Shell from '@/components/Shell.vue'

export default {
  name: 'App',
  components: {
    Shell
  }
}
</script>

<style lang="scss">

body {
  scroll-behavior: smooth;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  scroll-behavior: smooth;

}
</style>
