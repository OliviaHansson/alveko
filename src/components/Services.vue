<template>
  <div class="services" id="services">
    <div class="services__intro">
      <h2>Våra Tjänster</h2>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod 
        tempor incididunt ut labore et dolore magna aliaboris nisi ut aliquip ex ea.
      </p>
    </div>
    <div class="services__row">
      <ServiceCard class="card"/>
      <ServiceCard class="card"/>
      <ServiceCard class="card"/>
    </div>
    <div class="services__row">
      <ServiceCard class="card"/>
      <ServiceCard class="card"/>
    </div>
    <div class="services__row">
      <ServiceCard class="card"/>
      <ServiceCard class="card"/>
      <ServiceCard class="card"/>
    </div>
    <!-- <div class="services__row">
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
    </div> -->
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
    
    &__intro {
      text-align: center;
      margin-bottom: 100px;
    }
    h2 {
      color: $headingsColor-dark;
      font-size: 2em;
      margin-bottom: 40px;
    }
    p {
      width: 50%;
      margin: 0 auto;
    }

    &__row {
      display: flex;
      flex-flow: row wrap;
      justify-content: center;
    }
    // &__row:nth-of-type(3) {
    //   justify-content: space-around;
    // }
  }
</style>