<template>
  <div id="jumbotron">
    <div class="container">
      <div class="row">
        <!-- Links -->
        <div class="col">
          <div class="row-between">
            <div class="col-3">
              <!-- Vertical Column -->
              <div class="row-column">
                <div class="col-8">
                  <h2>DC COMICS</h2>
                  <ul>
                    <li
                      v-for="(DcComicsLink, index) in DcComicsLinks"
                      :key="index"
                    >
                      <a :href="DcComicsLink.url">{{ DcComicsLink.name }}</a>
                    </li>
                  </ul>
                </div>
                <div class="col-4">
                  <h2>SHOP</h2>
                  <ul>
                    <li v-for="(ShopLink, index) in ShopLinks" :key="index">
                      <a :href="ShopLink.url">{{ ShopLink.name }}</a>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="col-3">
              <!-- DC Column -->
              <h2>DC</h2>
              <ul>
                <li v-for="(DcLink, index) in DcLinks" :key="index">
                  <a :href="DcLink.url">{{ DcLink.name }}</a>
                </li>
              </ul>
            </div>
            <div class="col-3">
              <!-- Sites Column -->
              <h2>SITES</h2>
              <ul>
                <li v-for="(SitesLink, index) in SitesLinks" :key="index">
                  <a :href="SitesLink.url">{{ SitesLink.name }}</a>
                </li>
              </ul>
            </div>
          </div>
        </div>

        <!-- Logo Dc -->
        <div class="col-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Jumbotron",
  data() {
    return {
      DcComicsLinks: [
        {
          name: "Characters",
          url: "#",
        },
        {
          name: "Comics",
          url: "#",
        },
        {
          name: "Movies",
          url: "#",
        },
        {
          name: "TV",
          url: "#",
        },
        {
          name: "Games",
          url: "#",
        },
        {
          name: "Videos",
          url: "#",
        },
        {
          name: "News",
          url: "#",
        },
      ],
      ShopLinks: [
        {
          name: "Shop DC",
          url: "#",
        },
        {
          name: "Shop DC Collectibles",
          url: "#",
        },
      ],
      DcLinks: [
        {
          name: "Term Of Use",
          url: "#",
        },
        {
          name: "Privacy Policy (New)",
          url: "#",
        },
        {
          name: "Ad Choices",
          url: "#",
        },
        {
          name: "Advertising",
          url: "#",
        },
        {
          name: "Jobs",
          url: "#",
        },
        {
          name: "Subscriptions",
          url: "#",
        },
        {
          name: "Talent Workshops",
          url: "#",
        },
        {
          name: "CPSC Certificates",
          url: "#",
        },
        {
          name: "Ratings",
          url: "#",
        },
        {
          name: "Shop Help",
          url: "#",
        },
        {
          name: "Contact Us",
          url: "#",
        },
      ],
      SitesLinks: [
        {
          name: "DC",
          url: "#",
        },
        {
          name: "MAD Magazine",
          url: "#",
        },
        {
          name: "DC Kids",
          url: "#",
        },
        {
          name: "DC Universe",
          url: "#",
        },
        {
          name: "DC Power Visa",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_mixins.scss";
@import "../assets/scss/_vars.scss";
#jumbotron {
  height: 370px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;

  .row {
    height: 320px;
    width: 100%;
    @include center("vertical");
    justify-content: space-between;

    .col {
      height: 100%;
      width: calc(100% / 2);
      @include center("column");

      .row-between {
        height: 100%;
        width: 70%;
        @include center("vertical");
        justify-content: start;

        .col-3 {
          height: 100%;
          width: calc(100% / 3);
          @include center("column");
          padding-top: 50px;
          color: white;

          .row-column {
            height: 100%;
            @include center("column");

            .col-8 {
              width: 100%;
              @include center("column");
              padding-bottom: 30px;
              color: white;
            }

            .col-4 {
              width: 100%;
              @include center("column");
              color: white;
            }
          }

          h2 {
            font-size: 18px;
            padding-bottom: 20px;
            font-family: Georgia, "Times New Roman", Times, serif;
          }

          li {
            line-height: 20px;
            a {
              color: grey;
            }
          }
        }
      }
    }

    .col-logo {
      height: 100%;
      width: calc(100% / 2);
      @include center("both");

      img {
        max-height: 550px;
      }
    }
  }
}
</style>