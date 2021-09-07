<template>
  <div id="jumbotron">
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="row-pe">
            <div class="col-3">
              <div class="row-column">
                <div class="col-8">
                  <h2>DC COMICS</h2>
                  <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                  </ul>
                </div>
                <div class="col-4">
                  <h2>SHOP</h2>
                  <ul>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="col-3">
              <h2>DC</h2>
              <ul>
                <li>Term Of Use</li>
                <li>Privacy policy (New)</li>
                <li>Ad Choices</li>
                <li>Advertising</li>
                <li>Jobs</li>
                <li>Subscriptions</li>
                <li>Talent Workshops</li>
                <li>CPSC Certificates</li>
                <li>Ratings</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
              </ul>
            </div>
            <div class="col-3">
              <h2>SITES</h2>
              <ul>
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>Dc Power Visa</li>
              </ul>
            </div>
          </div>
        </div>
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
};
</script>

<style scoped>
#jumbotron {
  height: 370px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

#jumbotron img {
  max-height: 550px;
}

#jumbotron h2 {
  font-size: 18px;
  padding-bottom: 20px;
  font-family: Georgia, "Times New Roman", Times, serif;
}

#jumbotron .col-3 li {
  line-height: 20px;
  color: grey;
}

.row {
  height: 320px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.row-pe {
  height: 100%;
  width: 70%;
  display: flex;
  align-items: center;
  justify-content: start;
}

.row-column {
  height: 100%;
  display: flex;
  flex-direction: column;
}

.col {
  height: 100%;
  width: calc(100% / 2);
  display: flex;
  flex-direction: column;
}

.col-logo {
  height: 100%;
  width: calc(100% / 2);
  display: flex;
  align-items: center;
  justify-content: center;
}

.col-3 {
  color: white;
  height: 100%;
  width: calc(100% / 3);
  display: flex;
  flex-direction: column;
  padding-top: 50px;
}

.col-8 {
  color: white;
  width: 100%;
  display: flex;
  flex-direction: column;
  padding-bottom: 30px;
}

.col-4 {
  color: white;
  width: 100%;
  display: flex;
  flex-direction: column;
}
</style>