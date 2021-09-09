<template>
  <footer id="footer">
    <div class="container">
      <div class="row">
        <div class="col-1">
          <input class="button" type="button" value="SIGN UP NOW!" />
        </div>
        <div class="col-2">
          <div class="text-blue">FOLLOW US</div>
          <ul>
            <li v-for="(socialIcon, index) in socialIcons" :key="index">
              <a href="#" class="social"
                ><img :src="socialIcon.image" :alt="socialIcon.name"
              /></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      socialIcons: [
        {
          name: "Facebook",
          image: require("../assets/img/footer-facebook.png"),
        },
        {
          name: "Twitter",
          image: require("../assets/img/footer-twitter.png"),
        },
        {
          name: "YouTube",
          image: require("../assets/img/footer-youtube.png"),
        },
        {
          name: "Pinterest",
          image: require("../assets/img/footer-pinterest.png"),
        },
        {
          name: "Periscope",
          image: require("../assets/img/footer-periscope.png"),
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
@import "../assets/scss/_mixins.scss";
#footer {
  position: relative;
  height: 117px;
  width: 100%;
  background-color: $Footer-Color;

  .row {
    height: 117px;
    width: 100%;
    @include center("vertical");
    justify-content: space-between;

    .col-1 {
      height: 100%;
      width: calc(100% / 2);
      @include center("vertical");
      justify-content: flex-start;

      .button {
        padding: 15px 25px;
        background-color: $Footer-Color;
        border: 2px solid $Principal-Color;
        color: white;
      }
    }

    .col-2 {
      height: 100%;
      width: calc(100% / 2);
      @include center("vertical");
      justify-content: flex-end;

      .text-blue {
        font-size: 25px;
        font-weight: 600;
        margin-right: 30px;
        color: $Principal-Color;
      }

      ul {
        display: flex;

        li {
          margin-right: 20px;
        }
      }
    }
  }
}
</style>