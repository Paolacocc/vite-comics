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
    <appMain />
    <AppFooter />
  
</template>

<style lang="scss">
@use "./style/general.scss"
</style>