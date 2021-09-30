<template>
  <div class="content">
    <Hero src="/images/jumbotron.jpg" alt="Jumbotron" height="20em" />
    <div class="container">
      <div class="title">
        <h2>Current Series</h2>
      </div>
      <Cards :array="cards" colls="6" />
      <div class="load-more">
        <h3>Load More</h3>
      </div>
    </div>
  </div>
</template>

<script>
import jsonCards from "./dc-comics.json";
import Hero from "./Hero.vue";
import Cards from "./Cards.vue";

export default {
  name: "Content",
  components: {
    Hero,
    Cards,
  },
  data() {
    return {
      cards: jsonCards,
    };
  },
  methods: {
    getCards() {
      fetch("weather.json")
        .then((response) => response.json())
        .then((data) => (this.weatherDataList = data));
    },
  },
};
</script>

<style scoped lang="scss">
@import "../scss/vars";

.content {
  background-color: $secondary-color;
  color: $white-color;

  .container {
    .title {
      position: relative;
      top: -2em;
      @include blue-shape;
    }
    .load-more {
      text-align: center;
      padding: 2em 0;
      h3 {
        display: inline-block;
        @include blue-shape;
        padding: 0.5em 4em;
      }
    }
  }
}
</style>