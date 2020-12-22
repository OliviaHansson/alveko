<template>
  <div class="shell">
    <Menubar />
    <Intro />
    <Services />
    <About />
    <Contact />
    <UpButton />
  </div>
</template>
<script>
import Menubar from '@/components/Menubar'
import Intro from '@/components/Intro'
import Services from '@/components/Services'
import About from '@/components/About'
import Contact from '@/components/Contact'
import UpButton from '@/components/UpButton'


export default {
  name: 'Shell',
  components: {
    Menubar,
    Intro,
    Services,
    About,
    Contact,
    UpButton
  },
}
</script>
<style lang="scss" scoped>
</style>