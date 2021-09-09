<template>
  <div id="nav-bar">
    <div class="container">
      <div class="content">
        <div class="logo">
          <a href="#"><img alt="DC Logo" src="../assets/img/dc-logo.png" /></a>
        </div>
        <div class="menu">
          <ul>
            <li v-for="(link, index) in links" :key="index + link.name">
              <a href="link.url" :class="{ active: link.current }">{{
                link.name
              }}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          name: "CHARCTERS",
          url: "#",
          current: false,
        },
        {
          name: "COMICS",
          url: "#",
          current: true,
        },
        {
          name: "MOVIES",
          url: "#",
          current: false,
        },
        {
          name: "TV",
          url: "#",
          current: false,
        },
        {
          name: "GAMES",
          url: "#",
          current: false,
        },
        {
          name: "COLLECTIBLES",
          url: "#",
          current: false,
        },
        {
          name: "VIDEOS",
          url: "#",
          current: false,
        },
        {
          name: "FANS",
          url: "#",
          current: false,
        },
        {
          name: "NEWS",
          url: "#",
          current: false,
        },
        {
          name: "SHOP",
          url: "#",
          current: false,
        },
      ],
    };
  },
  computed: {
    sortedLinks() {
      const linksCopy = [...this.links];

      return linksCopy.sort((a, b) => {
        if (a.name > b.name) return 1;
        if (a.name < b.name) return -1;
        else return 0;
      });
    },
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_mixins.scss";
@import "../assets/scss/_vars.scss";
#nav-bar {
  height: 120px;
  width: 100%;
  background-color: $Header-Color;

  .content {
    @include center("between");
    height: 120px;

    img {
      height: 120px;
      padding: 20px;
    }

    ul {
      @include center("horizontal");
      padding: 0;

      li {
        height: 120px;
        line-height: 120px;
        font-weight: bold;

        a {
          padding: 10px;
          padding-bottom: 50px;
        }
      }
    }
  }
}
</style>