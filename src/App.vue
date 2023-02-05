<template>
  
  <div>
    <header-app></header-app>
    <footer-app></footer-app>
  </div>
</template>
<script>
import HeaderApp from './components/HeaderApp.vue';
import FooterApp from './components/FooterApp.vue';
export default {
  components: {
    HeaderApp,
    FooterApp,
  },
  name: "App",
}
</script>
<style src="./assets/sass/style.scss" lang="scss">

</style>