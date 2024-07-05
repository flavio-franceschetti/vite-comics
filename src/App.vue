<script>
import HeaderApp from "./components/HeaderApp.vue";
import AppMainContent from "./components/AppMainContent.vue";
import AppIconSection from "./components/AppIconSection.vue";
import AppFirtstFooter from "./components/AppFirtstFooter.vue";

export default {
  name: "App",
  components: {
    HeaderApp,
    AppMainContent,
    AppIconSection,
    AppFirtstFooter,
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
  <div class="icon-section">
    <AppIconSection />
  </div>
  <!-- footer -->
  <footer>
    <!-- firstfooter -->
    <div class="first-footer">
      <AppFirtstFooter />
    </div>
    <!-- second footer -->
    <div class="second-footer"></div>
  </footer>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
