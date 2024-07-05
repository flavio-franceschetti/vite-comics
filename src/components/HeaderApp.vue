<script>
export default {
  name: "HeaderApp",
};
</script>

<template>
  <div class="container">
    <!-- logo -->
    <div class="logo">
      <img src="/public/img/dc-logo.png" alt="" />
    </div>
    <!-- nav -->
    <div class="nav-bar">
      <ul>
        <li>
          <a href="#">Characters</a>
        </li>
        <li>
          <a href="#">Comics</a>
        </li>
        <li>
          <a href="#">Movies</a>
        </li>
        <li>
          <a href="#">tv</a>
        </li>
        <li>
          <a href="#">Games</a>
        </li>
        <li>
          <a href="#">Characters</a>
        </li>
        <li>
          <a href="#">Comics</a>
        </li>
        <li>
          <a href="#">Movies</a>
        </li>
        <li>
          <a href="#">tv</a>
        </li>
        <li>
          <a href="#">Games</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "/src/styles/partial/mixins" as *;
@use "/src/styles/partial/variables" as *;

.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 150px;
  background-color: #fff;
  padding: 20px 0;
}

.nav-bar {
  ul {
    list-style: none;
    display: flex;
    gap: 15px;
  }

  li a {
    text-transform: uppercase;
    font-weight: bold;
  }
}
</style>
