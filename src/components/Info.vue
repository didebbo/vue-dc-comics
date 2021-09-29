<template>
  <div>
    <div class="container">
      <ul>
        <li v-for="(item, index) in items" :key="index">
          <img :src="`images/${item.icon}`" :alt="item.text" />
          <p>{{ item.text }}</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Info",
  data() {
    return {
      items: [
        {
          text: "Digital Comics",
          icon: "buy-comics-digital-comics.png",
        },
        {
          text: "DC Merchandise",
          icon: "buy-comics-merchandise.png",
        },
        {
          text: "Subscription",
          icon: "buy-comics-subscriptions.png",
        },
        {
          text: "Comic Shop Locator",
          icon: "buy-comics-shop-locator.png",
        },
        {
          text: "DC Power Visa",
          icon: "buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "@/scss/sections/info";
</style>