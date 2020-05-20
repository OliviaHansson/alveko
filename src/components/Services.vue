<template>
  <div class="services">
    <h2>Våra Tjänster</h2>
    <p class="services__offering">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod 
      tempor incididunt ut labore et dolore magna aliaboris nisi ut aliquip ex ea.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod 
      tempor incididunt ut labore et dolore magna aliaboris nisi ut aliquip ex ea.
    </p>
    <div class="services__row">
      <ServiceCard class="card" :isInverted='false'/>
      <ServiceCard class="card" :isInverted='true'/>
      <ServiceCard class="card" :isInverted='false'/>
    </div>
    <div class="services__row">
      <ServiceCard class="card" :isInverted='false'/>
      <ServiceCard class="card" :isInverted='true'/>
    </div>
    <div class="services__row">
      <ServiceCard class="card" :isInverted='true'/>
      <ServiceCard class="card" :isInverted='false'/>
    </div>  
  </div>
</template>
<script>
import ServiceCard from '@/components/ServiceCard'

export default {
  name: 'Services',
  components: {
    ServiceCard
  }
}
</script>
<style lang="scss" scoped>
  .services {
    @include base(#D8D1CF);
    min-height: 700px;

    h2 {
      color: $headingsColor-dark;
      font-size: 2em;
    }
    &__offering {
      width: 50%;
    }

    &__row {
      display: flex;
      flex-flow: row wrap;
      justify-content: center;
    }
    &__row:nth-of-type(3) {
      justify-content: space-around;
    }
  }
</style>