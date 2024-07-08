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
    <div>{{ details.series }}</div>
  </div>
</template>

<style lang="scss" scoped></style>
