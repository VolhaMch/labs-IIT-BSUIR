<template>
  <div id="app">
    <HeaderComponent
      v-if="$route.name != 'login' && $route.name != '404'"
    ></HeaderComponent>
    <router-view></router-view>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import HeaderComponent from "./components/layout/HeaderComponent.vue";
// import "@/assets/style/global.scss";
export default {
  name: "app",
  components: {
    HeaderComponent,
  },
};
</script>

<style></style>
