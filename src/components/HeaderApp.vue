<script>
export default {
  name: "HeaderApp",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
  methods: {
    // metodo per la classe active nella navigazione
    clickNavActive(indice) {
      // ciclo tutti i link e al click rendo tutti i valori di current false
      this.links.forEach((link) => {
        link.current = false;
      });
      // e rendo il valore di current del link cliccato true
      this.links[indice].current = true;
    },
  },
};
</script>

<template>
  <div class="container">
    <!-- logo -->
    <div class="logo">
      <img src="/public/img/dc-logo.png" alt="dc logo" />
    </div>
    <!-- nav -->
    <div class="nav-bar">
      <ul>
        <li
          @click="clickNavActive(index)"
          v-for="(link, index) in links"
          :key="index"
        >
          <a :class="link.current ? 'active' : ''" href="#">{{ link.text }}</a>
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
  // padding: 20px 0;
  @include container90;
}

.nav-bar {
  height: 100%;

  ul {
    list-style: none;
    display: flex;
    height: 100%;
    gap: 15px;
  }

  li a {
    display: inline-block;
    text-transform: uppercase;
    font-weight: bold;
    align-content: center;
    height: 100%;
  }
}

.active {
  @include activeNavElement;
}
</style>
