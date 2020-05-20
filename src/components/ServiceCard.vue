<template>
  <div class="card" :class="{inverted : isInverted }">
    <h4 class="card__heading">Personaladministration/HR:</h4>
    <p class="card__text">Hjälp med att upprätta:</p>
    <ul class="card__text">
      <li>Anställningsavtal</li>
      <li>Permitteringar</li>
      <li>Uppsägningar</li>
      <li>Föräldraledighet, tjänstledighet mm.</li>
      <li>Fackliga förhandlingar</li>
    </ul>
  </div>
</template>
<script>

export default {
  name: 'ServiceCard',
  props: {
    isInverted: {
      type: Boolean,
      default: false
    }
  }
}
</script>
<style lang="scss" scoped>
  .card {
    width: 280px;
    height: 280px;
    margin: 40px;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    // padding: 30px;

    &__heading {
      color: pink;
      text-align: center;
      margin: 20px;
      // font-weight: 700;
      font-size: 1.2em;
      // letter-spacing: 1px;
    }
    &__text {
      margin: 20px;
      // padding-top: 30px;
      // padding-left: 30px;
    }
  }
  .inverted {
      background-color: $backgroundColor-darkPink;
    }
</style>