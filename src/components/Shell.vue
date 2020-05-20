<template>
  <div class="shell">
    <Menubar />
    <Intro />
    <Services />
    <About />
    <Contact />
  </div>
</template>
<script>
import Menubar from '@/components/Menubar'
import Intro from '@/components/Intro'
import Services from '@/components/Services'
import About from '@/components/About'
import Contact from '@/components/Contact'

export default {
  name: 'Shell',
  components: {
    Menubar,
    Intro,
    Services,
    About,
    Contact
  },
}
</script>
<style lang="scss" scoped>
.shell {
}
</style>