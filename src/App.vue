<script>
import HeaderApp from "./components/HeaderApp.vue";
import AppMainContent from "./components/AppMainContent.vue";
import AppIconSection from "./components/AppIconSection.vue";
import AppFirtstFooter from "./components/AppFirtstFooter.vue";
import AppSecondFooter from "./components/AppSecondFooter.vue";

export default {
  name: "App",
  components: {
    HeaderApp,
    AppMainContent,
    AppIconSection,
    AppFirtstFooter,
    AppSecondFooter,
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
    <div class="second-footer">
      <AppSecondFooter />
    </div>
  </footer>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
