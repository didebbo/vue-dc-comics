<template>
  <div class="card">
    <div class="thumb">
      <img :src="card.thumb" :alt="card.series" />
    </div>
    <p>
      {{ card.series }}
    </p>
  </div>
</template>
<script>
export default {
  name: "Card",
  props: ["card"],
};
</script>

<style scoped lang="scss">
.card {
  display: flex;
  flex-direction: column;
  width: (100% / 6);
  padding: 1em;

  .thumb {
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }

  p {
    margin-top: 0.5em;
    text-transform: uppercase;
  }
}
</style>