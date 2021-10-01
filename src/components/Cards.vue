<template>
  <div class="cards">
    <Card v-for="(card, index) in array" :key="index" :card="card" colls="6" />
  </div>
</template>

<script>
import Card from "./Card.vue";

export default {
  name: "Cards",
  props: ["array"],
  components: {
    Card,
  },
};
</script>

<style scoped lang="scss">
.cards {
  display: flex;
  flex-wrap: wrap;
}
</style>