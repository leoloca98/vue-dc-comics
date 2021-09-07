<template>
  <div id="nav-bar-menu">
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="row-pe">
            <div class="col-4">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
            </div>
            <div class="col-8">
              <span>DIGITAL COMICS</span>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="row-pe">
            <div class="col-4">
              <img src="../assets/img/buy-comics-merchandise.png" alt="" />
            </div>
            <div class="col-8">
              <span>DC MERCHANDISE</span>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="row-pe">
            <div class="col-4">
              <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
            </div>
            <div class="col-8">
              <span>SUBSCRIPTION</span>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="row-pe">
            <div class="col-4">
              <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
            </div>
            <div class="col-8">
              <span>COMIC SHOP LOCATOR</span>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="row-pe">
            <div class="col-4">
              <img src="@/assets/img/buy-dc-power-visa.svg" alt="" />
            </div>
            <div class="col-8">
              <span>CD POWER VISA</span>
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
};
</script>

<style scoped>
#nav-bar-menu {
  height: 150px;
  width: 100%;
  background-color: rgb(2, 130, 249);
  position: relative;
}

#nav-bar-menu img {
  max-height: 50px;
  max-width: 50px;
  padding: 0;
  margin: 0;
}

.row {
  height: 150px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.row-pe {
  height: 100%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.col {
  height: 100%;
  width: calc(100% / 5);
}

.col-8 {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: start;
}
.col-4 {
  height: 100%;
  width: calc(100% / 3);
  display: flex;
  align-items: center;
  justify-content: center;
}

span {
  color: white;
}
</style>