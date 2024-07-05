<script>
import HeaderApp from "./components/HeaderApp.vue";

export default {
  name: "App",
  components: {
    HeaderApp,
  },
};
</script>

<template>
  <!-- header -->
  <header class="container">
    <HeaderApp />
  </header>
  <!-- main -->
  <main class="content-section">
    <div class="container"></div>
  </main>
  <!-- icons section -->
  <div class="icon-section">
    <div class="container"></div>
  </div>
  <!-- footer -->
  <footer>
    <!-- firstfooter -->
    <div class="first-footer">
      <div class="container"></div>
    </div>
    <!-- second footer -->
    <div class="second-footer">
      <div class="container"></div>
    </div>
  </footer>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
