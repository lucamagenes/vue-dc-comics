<template>
  <div id="app">
    <HeaderComponent />
    <!-- header -->

    <MainComponent />
    <!-- main component -->

    <FooterComponent />
    <!-- footer component -->
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/common.scss";
</style>
