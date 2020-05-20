<template>
  <div class="about">
    <h2>About</h2>
  </div>
</template>
<script>
export default {
  name: 'About'
}
</script>
<style lang="scss" scoped>
  .about {
    border: 1px solid red;
    min-height: 700px;
    @include base(#14272D);
    
    h2 {
      color: pink;
    }
  }
</style>