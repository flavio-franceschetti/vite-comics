<script>
export default {
  name: "AppIconSection",
  data() {
    return {
      icons: [
        {
          image: "buy-comics-digital-comics.png",
          alt: "DIGITAL COMICS",
          text: "Digital comics",
        },
        {
          image: "buy-comics-merchandise.png",
          alt: "DC MERCHANDAISE",
          text: "DC Merchandaise",
        },
        {
          image: "buy-comics-subscriptions.png",
          alt: "SUBSCRIPTION",
          text: "Subscription",
        },
        {
          image: "buy-comics-shop-locator.png",
          alt: "COMIC SHOP LOCATOR",
          text: "Comic Shop Locator",
        },
        {
          image: "buy-dc-power-visa.svg",
          alt: "DC POWER VISA",
          text: "Dc Power Visa",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container">
    <div v-for="(icon, index) in icons" :key="index" class="icon-element">
      <img :src="`/img/${icon.image}`" :alt="icon.alt" />
      <span>{{ icon.text }}</span>
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
  gap: 10;
}

.icon-element {
  display: flex;
  align-items: center;
  gap: 5px;

  img {
    width: 40px;
  }

  span {
    color: #fff;
    text-transform: uppercase;
  }
}

img[alt*="COMIC SHOP LOCATOR"] {
  width: 30px;
}
</style>
