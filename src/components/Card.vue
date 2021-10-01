<template>
  <div class="card" :style="`width: calc(100% / ${colls})`">
    <div class="thumb">
      <a href="#">
        <img :src="card.thumb" :alt="card.series" />
      </a>
    </div>
    <a href="#">
      {{ card.series }}
    </a>
  </div>
</template>
<script>
export default {
  name: "Card",
  props: ["card", "colls"],
};
</script>

<style scoped lang="scss">
@import "../scss/libs";

.card {
  display: flex;
  flex-direction: column;
  // width: (100% / 6);
  padding: 1em;

  .thumb {
    a {
      display: flex;

      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
    }
  }

  a {
    margin-top: 0.5em;
    text-transform: uppercase;
    text-decoration: none;
    color: $white-color;
  }
}
</style>