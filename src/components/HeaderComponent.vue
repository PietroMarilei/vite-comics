<script>
export default {
  data() {
    return {
      greeting: 'Hello World!'
    }
  },
  methods: {

  },
}
</script>

<template>
    <!-- header -->
   <header class="">
    <div class="my_left_header">
      <img src="../assets/img/dc-logo.png" alt="logo">
    </div>
    <div class="my_right_header">
      <a class="active" href="#">Characters</a>
      <a href="#">Comics</a>
      <a href="#">Movies</a>
      <a href="#">Tv</a>
      <a href="#">Games</a>
      <a href="#">Collectibles</a>
      <a href="#">Videos</a>
      <a href="#">Fans</a>
      <a href="#">News</a>
      <a href="#">Shop</a>
    </div>
  </header>

</template>

<style lang="scss" scoped>
  @use "../assets/scss/partials/variables.scss" as *;
  @use "../assets/scss/partials/reset.scss" as *;

    header {       
        background-color: $secondary-color-white;
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        font-weight: bold;
        font-stretch: condensed;
        padding: 1rem;
        text-align: center;

      a {
        text-transform: uppercase;
        padding: 0.3rem;
      }
      // 💢 hover non va 
      // & :hover,
       & .active {
        border-bottom: 4px solid rgb(0, 166, 255);
      }
      img {
        padding:0 1rem;
        width: 120px;
      }
    }

    
</style>