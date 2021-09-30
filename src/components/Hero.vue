<template>
  <div class="hero">
    <img :src="src" :alt="alt" :style="`height:${height}`" />
  </div>
</template>

<script>
export default {
  name: "Hero",
  props: ["src", "alt", "height"],
};
</script>

<style scoped lang="scss">
.hero {
  display: flex;
  width: 100%;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top center;
  }
}
</style>