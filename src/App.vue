<script>
import HeaderApp from "./components/HeaderApp.vue";
import AppMainContent from "./components/AppMainContent.vue";

export default {
  name: "App",
  components: {
    HeaderApp,
    AppMainContent,
  },
};
</script>

<template>
  <!-- header -->
  <header>
    <HeaderApp />
  </header>
  <!-- main -->
  <main class="content-section">
    <AppMainContent />
  </main>
  <!-- icons section -->
  <div class="icon-section"></div>
  <!-- footer -->
  <footer>
    <!-- firstfooter -->
    <div class="first-footer"></div>
    <!-- second footer -->
    <div class="second-footer"></div>
  </footer>
</template>

<style lang="scss">
@use "./styles/general.scss";

.content-section {
  background-color: rgb(28, 28, 28);
}
</style>
