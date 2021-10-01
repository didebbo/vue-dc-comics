<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import "./scss/libs";

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "PT Sans Narrow", sans-serif;
  font-weight: 400;
  font-size: 1rem;
  text-transform: uppercase;
  cursor: default;
}

ul {
  list-style: none;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}
</style>
