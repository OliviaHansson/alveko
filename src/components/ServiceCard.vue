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
    width: 300px;
    height: 300px;
    margin: 40px;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);

    &__heading {
      color: black;
      text-align: center;
      margin: 20px;
      font-size: 1.2em;
    }
    &__text {
      margin: 20px;
    }
  }
  .inverted {
    background-color: $backgroundColor-darkPink;
  }
</style>