<script>
export default {
  name: "AppMainContent",
};
</script>

<template>
  <div class="container">
    <h1>--> CONTENT GOES HERE <--</h1>
  </div>
</template>

<style lang="scss" scoped>
@use "/src/styles/partial/mixins" as *;
@use "/src/styles/partial/variables" as *;

.container {
  @include container90;
  color: #fff;
  padding: 50px 0;
}
</style>
