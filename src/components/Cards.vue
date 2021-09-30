<template>
  <div class="cards">
    <Card v-for="(card, index) in array" :key="index" :card="card" />
  </div>
</template>

<script>
import Card from "@/components/Card.vue";

export default {
  name: "Cards",
  props: ["array", "colls"],
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