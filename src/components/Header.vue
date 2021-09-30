<template>
  <header>
    <div class="container">
      <a class="logo" href="#">
        <img src="images/dc-logo.png" alt="DC Logo" />
      </a>
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
@import "@/scss/vars";

header {
  .container {
    display: flex;
    justify-content: space-between;

    .logo {
      padding: 0.8em 0;
      display: flex;

      img {
        height: 4em;
      }
    }
  }

  nav {
    display: flex;
    ul {
      display: flex;

      li {
        display: flex;
        align-items: center;
        margin: 0 0.8em;

        &.active {
          position: relative;

          a {
            color: $primary-color;
          }

          &::after {
            position: absolute;
            display: block;
            content: "";
            width: 100%;
            height: 0.2em;
            bottom: 0;
            background-color: $primary-color;
          }
        }

        a {
          text-decoration: none;
          font-weight: 700;
          font-size: 1.1em;
          text-transform: uppercase;
          color: $secondary-color;
        }
      }
    }
  }
}
</style>
