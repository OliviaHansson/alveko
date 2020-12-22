<template>
  <div class="about" id="about">
    <img class="about__img" src="@/assets/images/group.png" alt="">
    <div class="about__container">
      <div class="about__one"> 
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
          sed do eiusmod tempor incididunt ut labore et dolore magna 
          aliaboris nisi ut aliquip ex ea.
        </p>
      </div>
      <div class="about__two"> 
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
          sed do eiusmod tempor incididunt ut labore et dolore magna 
          aliaboris nisi ut aliquip ex ea.
        </p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'About'
}
</script>
<style lang="scss" scoped>
  .about {
    min-height: 700px;
    @include base(#14272D);

    &__img {
      width: 500px;
      margin: 20px auto 100px auto;
    }
    
    &__container {
      width: 70%;
      margin: 0 auto;
      
      p {
        color: black;
        font-size: 1.5em;
      }
    }
    &__one {
      width: 60%;
      margin: 50px;
      margin-left: 50px;
    }
    &__two {
      width: 60%;
      margin: 50px;
      margin-left: 300px;

      p {
        text-align: right;
      }
    }
  }
</style>