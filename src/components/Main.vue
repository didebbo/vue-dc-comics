<template>
  <main>
    <Content />
  </main>
</template>

<script>
import Content from "@/components/Content.vue";

export default {
  name: "Main",
  components: {
    Content,
  },
};
</script>

<style scoped lang="scss">
@import "@/scss/sections/main";
</style>