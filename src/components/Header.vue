<template>
  <header>
    <div class="container">
      <div class="logo">
        <a href="#">
          <img src="images/dc-logo.png" alt="DC Logo" />
        </a>
      </div>
      <nav>
        <ul>
          <li
            v-for="(link, index) in nav"
            :key="index"
            :class="{ active: link.active }"
          >
            <a :href="link.url"> {{ link.text }} </a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      nav: [
        {
          text: "Characters",
          url: "#",
          active: false,
        },
        {
          text: "Comics",
          url: "#",
          active: true,
        },
        {
          text: "Movies",
          url: "#",
          active: false,
        },
        {
          text: "TV",
          url: "#",
          active: false,
        },
        {
          text: "Games",
          url: "#",
          active: false,
        },
        {
          text: "Collectables",
          url: "#",
          active: false,
        },
        {
          text: "Videos",
          url: "#",
          active: false,
        },
        {
          text: "Fans",
          url: "#",
          active: false,
        },
        {
          text: "News",
          url: "#",
          active: false,
        },
        {
          text: "Shop",
          url: "#",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "@/scss/sections/header";
</style>
