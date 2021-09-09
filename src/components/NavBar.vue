<template>
  <div id="nav-bar-menu">
    <div class="container">
      <div class="row">
        <div v-for="(link, index) in links" :key="index" class="col">
          <div class="row-pe">
            <div class="col-4">
              <img :src="link.image" :alt="link.text" />
            </div>
            <div class="col-8">
              <span>{{ link.text }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      links: [
        {
          text: "DIGITAL COMICS",
          image: require("../assets/img/buy-comics-digital-comics.png"),
        },
        {
          text: "DC MERCHANDISE",
          image: require("../assets/img/buy-comics-merchandise.png"),
        },
        {
          text: "SUBSCRIPTIONS",
          image: require("../assets/img/buy-comics-subscriptions.png"),
        },
        {
          text: "COMIC SHOP LOCATOR",
          image: require("../assets/img/buy-comics-shop-locator.png"),
        },
        {
          text: "CD POWER VISA",
          image: require("../assets/img/buy-dc-power-visa.svg"),
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
@import "../assets/scss/_mixins.scss";
#nav-bar-menu {
  height: 150px;
  width: 100%;
  background-color: $Principal-Color;
  position: relative;

  .row {
    height: 150px;
    width: 100%;
    @include center("vertical");
    justify-content: space-between;

    .col {
      height: 100%;
      width: calc(100% / 5);

      .row-pe {
        height: 100%;
        width: 100%;
        @include center("both");

        .col-4 {
          height: 100%;
          width: calc(100% / 3);
          @include center("both");

          img {
            max-height: 50px;
            max-width: 50px;
            padding: 0;
            margin: 0;
          }
        }

        .col-8 {
          height: 100%;
          @include center("vertical");
          justify-content: start;

          span {
            color: white;
          }
        }
      }
    }
  }
}
</style>