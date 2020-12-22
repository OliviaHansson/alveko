<template>
  <div class="menu">
    <div class="menu__navbar">
      <img @click="scrollToTop()" class="menu__logo" src="@/assets/images/logo.png" alt="Alveko logga">
      <ul class="menu__links" :class="{menu__links__open : mobileMenuOpen}"> 
        <li><a href="#services" class="menu__link">Våra tjänster</a></li>
        <li><a href="#about" class="menu__link">Om oss</a></li>
        <li><a href="#contact" class="menu__link">Kontakt</a></li>
      </ul>
      <div class="menu__icon" @click="toggleMenu()">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Menubar',
  data: function () {
    return {
      mobileMenuOpen: false
    }
  },
  methods: {

    scrollToTop() {
      // For Safari
      document.body.scrollTop = 0;
      // For Chrome, Firefox, IE and Opera
      document.documentElement.scrollTop = 0;
    },
  
    toggleMenu() {
      console.log('toggle', this.mobileMenuOpen)
      this.mobileMenuOpen = !this.mobileMenuOpen
    }
  }
}
</script>
<style lang="scss" scoped>
  .menu {
    // min-height: 8vh;
    width: calc(100% - 80px);
    padding: 0 40px;
    background-color: black;
    // border: 1px solid white;

    // @include tablet {
      // width: 90%;
      // min-height: 20vh;
    // }

    &__navbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    &__logo {
      width: 150px;
      // @include tablet {
      //   width: 180px;
      // }
    }
    &__links {
      display: none;
      width: 60%;
      justify-content: space-around;

      @include tablet {
        display: flex;
      }
      &__open{
        display: block;
      }
    }
    &__link {
      position: relative;
      font-size: 1.2em;
      color: white;
      font-family: $breadTypo;
    }

    // link hover animation
    &__link:after {
      content: '';
      position: absolute;
      width: 0; height: 2px;
      display: block;
      margin-top: 5px;
      right: 0;
      background: $headingsColor-light;
      transition: width .5s ease;
      -webkit-transition: width .5s ease;
      opacity: 80%;
    }
    &__link:hover:after {
      width: 100%;
      left: 0;
      background: $headingsColor-light;
    }

    // mobile menu icon
    &__icon {
      span {
        display: block;
        width: 50px;
        height: 2px;
        margin-bottom: 8px;
        background-color: $headingsColor-light;
      }
      span:nth-child(2){
        width: 40px;
      }
      @include tablet {
        display: none;
      }

    }
  }
</style>