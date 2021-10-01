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
@import "../scss/libs";
.hero {
  position: relative;
  display: flex;
  width: 100%;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top center;
  }

  &:after {
    position: absolute;
    display: block;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    content: "";
    background-color: $primary-color;
    opacity: 0.4;
  }
}
</style>