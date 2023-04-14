<script>
import appHeader from "./components/appHeader.vue";
import appMain from "./components/appMain.vue";
import AppFooter from "./components/AppFooter.vue"

export default {
  components: {
    appHeader,
    appMain,
    AppFooter
  },
  data() {
    return {
      
    }
  }
}
</script>

<template>
  
    <appHeader />
    <img class="banner-img" src="./assets/img/jumbotron.jpg" alt="">
    <appMain />
    <AppFooter />
  
</template>

<style lang="scss">
@use "./style/general.scss";
.banner-img {
  width: 100%;
  height: 300px;
  object-fit: cover;
}
</style>