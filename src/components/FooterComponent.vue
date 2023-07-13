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
    <!-- footer template -->
   <footer>
    <div class="my_blue_section">
      <div class="my_item">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="item">
         <p>Digital Comics</p>
      </div>
       <div class="my_item">
        <img src="../assets/img/buy-comics-merchandise.png" alt="item">
         <p>Digital Comics</p>
      </div>
       <div class="my_item">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="item">
         <p>Digital Comics</p>
      </div>
       <div class="my_item">
        <img id="gps_logo" src="../assets/img/buy-comics-shop-locator.png" alt="item">
         <p>Digital Comics</p>
      </div>
       <div class="my_item">
        <img  src="../assets/img/buy-dc-power-visa.svg" alt="item">
         <p>Digital Comics</p>
      </div>
    </div>
  </footer>

</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as*;
   
    .my_blue_section {
      display: flex;
      justify-content: space-around;
      align-items: center;
      padding: 2rem;
      background-color:$blue_banner ;
      font-stretch: condensed;
      text-transform: uppercase;
    };
    #gps_logo {
      width: 40px;
    };
    .my_item {
      display: flex;
      align-items: center;
      color: $secondary-color-white;


      img {
        width: 50px;
        padding:  0.5rem;
      }

      p {
        padding: 0.5rem;
      }
    }
</style>