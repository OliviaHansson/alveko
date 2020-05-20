<template>
  <div class="menu">
    <div class="menu__navbar">
      <img class="menu__logo" src="@/assets/images/logo.png" alt="Alveko logga">
      <ul class="menu__links"> 
        <li><a href="#" class="menu__link">Våra tjänster</a></li>
        <li><a href="#" class="menu__link">Om oss</a></li>
        <li><a href="#" class="menu__link">Kontakt</a></li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Menubar'
}
</script>
<style lang="scss" scoped>
  .menu {
    min-height: 20vh;
    width: 90%;
    margin: 0 auto;

    &__navbar {
      display: flex;
      align-items: center;
      justify-content: space-between;

      p {
        color: $headingsColor-light;
        font-size: 1.3em;
        letter-spacing: 2px;
      }
    }
    &__logo {
      width: 180px;
    }
    &__links {
      display: flex;
      width: 60%;
      justify-content: space-around;
    }
    &__link {
      position: relative;
      font-size: 20px;
      color: $headingsColor-light;
      font-family: $breadTypo;
    }
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
  }
</style>