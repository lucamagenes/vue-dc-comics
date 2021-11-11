<template>
  <div id="app">
    <HeaderComponent />
    <!-- header -->
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import HeaderComponent from "./components/HeaderComponent.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/common.scss";
</style>
