<script>
import BlueBarComponent from './BlueBarComponent.vue';
export default {
    components: [
        BlueBarComponent
    ],
    data() {
        return {
            greeting: "Hello World!"
        };
    },
    methods: {},
    components: { BlueBarComponent }
}
</script>

<template>
    <!-- footer template -->
   <footer>
    <BlueBarComponent/>
    
    <div class="my_jumbo_footer">

      <div class="my_footer_left">
        <div class="col-4 my_comics">
          <h3>DC COMICS</h3>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
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
            <li>Term of Use</li>
            <li>Privacy Policy</li>
            <li>Ad Choiches</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshop</li>
            <li>CPSC Certificates</li>
            <li>Rates</li>
            <li>Shop Help</li>
            <li>Contact us</li>
          </ul>
        </div>
        <div class="col-4 my_sites">
          <h3>SITES</h3>
          <ul>
            <li>DC</li>
            <li>Mad magazines</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
            
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
          padding: 0.2rem 0;
          font-size: 0.7rem;
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
        font-stretch:  semi-condensed;
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
          font-stretch:  semi-condensed;
          padding: 0 1rem;
        }
        a {
          padding: 0 0.3rem;
        }
      }
    }
</style>