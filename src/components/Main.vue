<template>
  <main>
    <Content />
    <Info />
  </main>
</template>

<script>
import Content from "./Content.vue";
import Info from "./Info.vue";

export default {
  name: "Main",
  components: {
    Content,
    Info,
  },
};
</script>

<style scoped lang="scss">
</style>