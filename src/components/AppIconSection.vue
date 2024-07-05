<script>
export default {
  name: "AppIconSection",
};
</script>

<template>
  <div class="container">
    <div class="icon-element">
      <img
        src="/public/img/buy-comics-digital-comics.png"
        alt="Digital comics"
      />
      <span>DIGITAL COMICS</span>
    </div>
    <div class="icon-element">
      <img src="/public/img//buy-comics-merchandise.png" alt="Digital comics" />
      <span>DC MERCHANDISE</span>
    </div>
    <div class="icon-element">
      <img
        src="/public/img/buy-comics-subscriptions.png"
        alt="Digital comics"
      />
      <span>SUBSCRIPTION</span>
    </div>
    <div class="icon-element">
      <img
        style="width: 25px"
        src="/public/img/buy-comics-shop-locator.png"
        alt="Digital comics"
      />
      <span>COMIC SHOP LOCATOR</span>
    </div>
    <div class="icon-element">
      <img src="/public/img/buy-dc-power-visa.svg" alt="Digital comics" />
      <span>DC POWER VISA</span>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "/src/styles/partial/mixins" as *;
@use "/src/styles/partial/variables" as *;

.container {
  @include container90;
  padding: 50px 30px;
  display: flex;
  justify-content: space-between;
}

.icon-element {
  display: flex;
  align-items: center;
  gap: 15px;

  img {
    width: 40px;
  }

  span {
    color: #fff;
  }
}
</style>
