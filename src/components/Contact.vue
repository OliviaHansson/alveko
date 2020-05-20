<template>
  <div class="contact">
    <h2>Contact</h2>
  </div>
</template>
<script>
export default {
  name: 'Contact'
}
</script>
<style lang="scss" scoped>
  .contact {
    border: 1px solid red;
    min-height: 700px;
    @include base(#D8D1CF);
    h2 {
      color: pink;
    }
  }
</style>