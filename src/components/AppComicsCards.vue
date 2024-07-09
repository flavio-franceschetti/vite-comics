<script>
export default {
  name: "AppComicsCards",
  props: {
    details: Object,
  },
};
</script>

<template>
  <div class="card">
    <div class="poster-img">
      <img :src="details.thumb" alt="Comic Thumb" />
    </div>
    <div class="series-title">{{ details.series }}</div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: calc(100% / 6 - 20px);
  aspect-ratio: 1 / 1;
}

.poster-img img {
  aspect-ratio: 1 / 1;
  object-fit: cover;
  object-position: top;
}

.series-title {
  font-size: 14px;
}
</style>
