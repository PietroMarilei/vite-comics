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
    <div class="my_jumbo_footer">

      <div class="my_footer_left">
        <div class="col-4 my_comics">
          <h3>DC COMICS</h3>
          <ul>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
          </ul>
          <div class="my_shop">
            <h3>MY SHOP</h3>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
          </div>
        </div>
        <div class="col-4 my_DC">
          <h3>DC </h3>
          <ul>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
          </ul>
        </div>
        <div class="col-4 my_sites">
          <h3>SITES</h3>
          <ul>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
            <li>Characters</li>
          </ul>
        </div>
      </div>

      <div class="my_footer_right">
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
    <div class="my_footer_footer">
      <button>
        <a href="#">
          SIGN UP NOW
        </a>
      </button>

      <div class="my_right_ff">
        <h3>FOLLOW US</h3>
        <a href="">
          <img src="../assets/img/footer-facebook.png" alt="">
        </a>
        <a href="">
          <img src="../assets/img/footer-twitter.png" alt="">
        </a>
        <a href="">
          <img src="../assets/img/footer-youtube.png" alt="">
        </a>
        <a href="">
          <img src="../assets/img/footer-pinterest.png" alt="">
        </a>
        <a href="">
          <img src="../assets/img/footer-periscope.png" alt="">
        </a>
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
      font-stretch: semi-condensed;
      text-transform: uppercase;
      font-weight: 600;

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
    };
    #gps_logo {
      width: 40px;
    };
    
    .my_jumbo_footer {
      background-image: url(../assets/img/footer-bg.jpg);
      object-fit: cover;
      padding: 0 8rem;
      height: 20rem;
      display: flex;
      justify-content: space-between;
      align-items: center;

      .my_footer_left {
        color: white;
        display: flex;
        justify-content: space-between;
        .col-4 {
          width: 8rem;
          margin: 0 auto;
        }
        h3 {
          font-weight: 700;
          padding: 1rem 0;
        }
        li {
          color: rgb(166, 166, 166);
        }
      }
      }

      .my_footer_right {
        img {
          height: 20rem;
          object-fit: cover;
          width: 500px;
          
        }
        
    }

    .my_footer_footer {
      background-color: $dark_grey;
      height: 6rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 0 8rem;

      button {
        font-weight: 800;
        font-stretch: condensed;
        color: $secondary-color-white;
        border: 2px solid $blue-banner;
        border-radius: 5px;
        padding: 0.8rem;
        cursor: pointer;
      }
      .my_right_ff {
        display: flex;
        align-items: center;

        h3 {
          color: $blue-banner;
          font-weight: 800;
          font-stretch: condensed;
          padding: 0 1rem;
        }
        a {
          padding: 0 0.3rem;
        }
      }
    }
</style>