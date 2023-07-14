<script>
import CardComponent from "../components/CardComponent.vue" ;

export default {
  components: {
    CardComponent,
  },
  data() {
    return {
      productsArr: [
            {
                "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                "price": "$19.99",
                "series": "Action Comics",
                "type": "comic book",
            },
            {
                "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                "price": "$3.99",
                "series": "American Vampire 1976",
                "type": "comic book",
            },
            {
                "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                "price": "$16.99",
                "series": "Aquaman",
                "type": "graphic novel",
            },
            {
                "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                "price": "$2.99",
                "series": "Batgirl",
                "type": "comic book",
            },
            {
                "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                "price": "$3.99",
                "series": "Batman",
                "type": "comic book",
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                "price": "$2.99",
                "series": "Batman Beyond",
                "type": "comic book",
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                "price": "$3.99",
                "series": "Batman/Superman",
                "type": "comic book",
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                "price": "$4.99",
                "series": "Batman/Superman Annual",
                "type": "comic book",
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                "price": "$5.99",
                "series": "Batman: The Joker War Zone",
                "type": "comic book",
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                "price": "$6.99",
                "series": "Batman: Three Jokers",
                "type": "comic book",
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                "price": "$4.99",
                "series": "Batman: White Knight Presents: Harley Quinn",
                "type": "comic book",
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                "price": "$16.99",
                "series": "Catwoman",
                "type": "graphic novel",
            },
],
    }
  },
  methods: {

  },
}
</script>

<template>
    <main>
      
      <div class="my_big_jumbo">
        
      </div>

      <div class="my_container">
        <h2>CURRENT SERIES</h2>

        <div div class="my_prod_shop">
        <!-- <div class="my_product" v-for="(singleProduct,i) in productsArr" :key="i">     
          <img :src="singleProduct.thumb" :alt="singleProduct.series">
          <h5 class="my_prod_title">{{singleProduct.series }}</h5>
        </div> -->
        <CardComponent
         v-for="(singleProduct,i) in productsArr" :key="i"
            :cardImg="singleProduct.thumb"
            :series="singleProduct.series" />  
            
         <h3>
            LOAD MORE
         </h3>
      </div>
      </div> 
      
    

   

  </main>

</template>

<style lang="scss" scoped>
  @use "../assets/scss/partials/variables.scss" as *;
  h2 {
    color:$secondary-color-white ;
    background-color: $blue-banner;
    padding: 0.5rem 1rem;
    display: inline-block;
    font-weight: 600;
    text-align: center;
     position: absolute;
   top: -20px;
  }
  main {
     .my_big_jumbo {
     background-image: url(../assets/img/jumbotron.jpg);
     height: 400px;
     background-position: top;
   }

   .my_container {
      max-width: 1200px;
      position: relative;
      padding: 2rem;

     .my_prod_shop {
        display: flex;
        justify-content: space-around;
        //align-items: center;
        flex-wrap: wrap;
        width: 90%;
        margin:0 auto;

      }
      h3 {
         color: $secondary-color-white;
         background-color: $blue-banner;
         padding: 0.5rem 3rem;
         font-size: medium;
      }
   }}
    
    
</style>