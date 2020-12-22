<template>
  <div class="contact" id="contact">
    <h2>Kontakta Oss</h2>
    <div class="contact__container">
      <div>
        <p>Alveko AB</p>
        <p>Flygkårsvägen 49</p>
        <p>184 56 Täby</p>
      </div>
      <div>
        <p>(+46) 705225570</p>
        <p>monica@alveko.se</p>
      </div>
    </div>

  </div>
</template>
<script>
export default {
  name: 'Contact'
}
</script>
<style lang="scss" scoped>
  .contact {
    min-height: 200px;
    @include base(#D8D1CF);
    background-color: black;

    h2 {
      text-align: center;
      font-size: 2.5em;
      color: $headingsColor-light;
    }

    &__container {
      width: 80%;
      margin: 40px auto;
      display: flex;
      justify-content: space-between;
      align-items: center;

      p {
        font-size: 1.5em;
        letter-spacing: 2px;
        margin-top: 15px;
        color: white;
      }
    }
  }
</style>