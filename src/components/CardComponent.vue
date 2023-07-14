<script>
export default {
  data() {
    return {     
    }
  },
  props: {
    cardImg: String,
    productTipe: String,
  },
  methods: {

  },
}
</script>

<template>
    
    <div class="my_product">             
          <img :src="cardImg" :alt="productTipe">
          <h5 class="my_prod_title">{{productTipe}}</h5>        
    </div>
 

</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
   
        .my_product {
          color: $secondary-color-white;
          padding: 0.5rem;
          width: calc(100% / 6);

          img {
             width: 100px;
             height: 100px;
              object-fit: cover;
      }
    }
    
    
</style>