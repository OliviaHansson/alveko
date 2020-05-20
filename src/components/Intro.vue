<template>
  <div class="intro">
    <div class="intro__container">
      <h1 class="intro__h1">ALVEKO</h1>
      <h2 class="intro__h2">redovisningsbyrå</h2>
      <p class="intro__text">Alveko den personliga byrån! Vi arbetar med små och medelstora bolag.
      Ni fokuserar på er kärnverksamhet, vi löser det administrativa. Vi skapar 
      anpassade lösningar utifrån era behov. Digitalt eller traditionellt, ni väljer.
      Varmt välkommen att höra av er!</p>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Intro'
}
</script>
<style lang="scss" scoped>
  .intro {
    @include base($backgroundColor-dark);
    min-height: 700px;
    margin-top: 80px;

    &__container {
      width: 60%;
      margin: 0 auto;
    }
    &__h1 {
    font-family: $logoTypo;
    color: $headingsColor-light;
    font-size: 7em;
    }
    &__h2 {
      font-family: $breadTypo;
      color: $headingsColor-light;
      font-size: 2em;
      margin-left: 130px;
      letter-spacing: 2px;
    }
    &__text {
      font-family: $breadTypo;
      margin-top: 40px;
      font-size: 1.4em;
      color: rgb(224, 222, 222);
      letter-spacing: 2px;
    }
  }
</style>