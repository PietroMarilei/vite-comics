<script>
export default {
  data() {
    return {     
    }
  },
  props: {
    cardImg: String,
    series: String,
  },
  methods: {

  },
}
</script>

<template>
    
    <div class="my_card">             
          <img :src="cardImg" :alt="series">
          <h5 class="my_prod_title">{{series}}</h5>        
    </div>
 

</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
   
        .my_card {
          color: $secondary-color-white;
          padding: 0.5rem;
          width: calc(100% / 6);
          

          img {
             width: 170px;
             height: 170px;
              object-fit: cover;
          }

          h5 {
            font-weight: lighter;
            text-transform: uppercase;
            padding: 0.5rem 0;
          }
            
          
    }
    
    
</style>