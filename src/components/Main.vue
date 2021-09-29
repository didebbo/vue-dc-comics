<template>
  <main>
    <Content />
    <Info />
  </main>
</template>

<script>
import Content from "@/components/Content.vue";
import Info from "@/components/Info.vue";

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