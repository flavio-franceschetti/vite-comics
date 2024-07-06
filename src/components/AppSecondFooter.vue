<script>
export default {
  name: "AppSecondFooter",
};
</script>
<template>
  <div class="container">
    <div class="singup-btn">
      <a href="#">SING-UP NOW!</a>
    </div>
    <div class="socials">
      <h3>FOLLOW US</h3>
      <div class="social-icons">
        <a href="#"
          ><img src="/public/img/footer-facebook.png" alt="facebook logo"
        /></a>
        <a href="#"
          ><img src="/public/img/footer-twitter.png" alt="twitter logo"
        /></a>
        <a href="#"
          ><img src="/public/img/footer-youtube.png" alt="youtube logo"
        /></a>
        <a href="#"
          ><img src="/public/img/footer-pinterest.png" alt="pinterest logo"
        /></a>
        <a href="#"
          ><img src="/public/img/footer-periscope.png" alt="periscope clogo"
        /></a>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use "/src/styles/partial/mixins" as *;
@use "/src/styles/partial/variables" as *;

.container {
  display: flex;
  justify-content: space-between;
  @include container90;
  padding: 50px 0;
}

.singup-btn {
  cursor: pointer;
  padding: 10px 25px;
  border: 2px solid $primary-blue-color;
  a {
    display: inline-block;
    color: #fff;
    font-weight: bold;
  }
}

.socials {
  display: flex;
  align-items: center;
  gap: 20px;

  h3 {
    color: $primary-blue-color;
  }
}

.social-icons {
  display: flex;
  gap: 10px;
}
</style>
