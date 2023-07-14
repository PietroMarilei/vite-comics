<script>
export default {
  data() {
    return {
      
    }
  }
}
</script>

<template>
   <div class="my_blue_section">

    <div class="my_container">
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
      
    </div>
</template>

<style lang="scss">
@use "../assets/scss/partials/variables.scss" as*;


.my_blue_section {
    
    
    background-color:$blue_banner ;
    
    .my_container {
        max-width: 1200px;
        font-stretch: semi-condensed;
        text-transform: uppercase;
        font-weight: 600;
        padding: 2rem ;
        display: flex;
        justify-content: space-between;
        align-items: center;

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
    }

      
    };
    #gps_logo {
      width: 40px;
    };
</style>