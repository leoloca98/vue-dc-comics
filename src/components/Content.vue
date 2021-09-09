<template>
  <div id="content">
    <div class="container">
      <div class="cdComics">
        <div class="currentSeries text-white">CURRENT SERIES</div>
        <div class="cdComics-list">
          <div
            v-for="(DcCard, index) in CdComicsCards"
            :key="index"
            class="card"
          >
            <figure>
              <img :src="DcCard.thumb" />
            </figure>
            <div class="nameDc">
              <span class="text-white uppercase">{{ DcCard.series }}</span>
            </div>
          </div>
        </div>
        <div>
          <button class="button text-white clickable">LOAD MORE</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Content",
  data() {
    return {
      CdComicsCards: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
#content {
  height: 600px;
  width: 100%;
  background-color: $Content-Color;

  .currentSeries {
    height: 40px;
    width: 180px;
    font-size: 17px;
    background-color: $Principal-Color;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    top: -3%;
    left: -38%;
  }

  .cdComics {
    height: 600px;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;

    .cdComics-list {
      height: 450px;
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      flex-wrap: wrap;

      .card {
        display: flex;
        flex-direction: column;
        height: 180px;
        width: 150px;
        margin: 15px;

        figure {
          height: 85%;
          width: 100%;

          img {
            height: 100%;
            width: 100%;
            object-fit: cover;
            object-position: top;
          }
        }

        .nameDc {
          display: flex;
          justify-content: flex-start;
          height: 15%;
          width: 100%;

          span {
            font-size: 11px;
            padding-top: 10px;
          }
        }
      }
    }

    .button {
      background-color: $Principal-Color;
      padding: 10px 50px;
      margin-top: 50px;
    }
  }
}
</style>