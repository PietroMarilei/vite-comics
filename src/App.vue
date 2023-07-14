<script >
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
  },
  data(){
    return {

    }
  }, 
  methods: {

  }
}
</script>

<template>
  <HeaderComponent/>

    <MainComponent/>

    <FooterComponent/>
  

</template>

<style lang="scss">
  @use "./assets/scss/main.scss" as *;
  @use "./assets/scss/partials/variables.scss" as *;
  @use "./assets/scss/partials/reset.scss" as *;
  
  body {
    background-color: lightslategray;
  }

  .my_container {
    //background-color: $secondary-color-white;
    margin: 0 auto;
    //max-width: 1200px;
  }
</style>
