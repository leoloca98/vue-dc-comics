<template>
  <footer id="footer">
    <div class="container">
      <div class="row">
        <div class="col-1">
          <input
            id="button"
            type="button"
            placeholder="SIGN UP NOW!"
            value="SIGN UP NOW!"
          />
        </div>
        <div class="col-2">
          <div class="txtb">FOLLOW US</div>
          <ul>
            <li>
              <img src="../assets/img/footer-facebook.png" alt="" />
            </li>
            <li>
              <img src="../assets/img/footer-twitter.png" alt="" />
            </li>
            <li>
              <img src="../assets/img/footer-youtube.png" alt="" />
            </li>
            <li>
              <img src="../assets/img/footer-pinterest.png" alt="" />
            </li>
            <li>
              <img src="../assets/img/footer-periscope.png" alt="" />
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
};
</script>

<style scoped>
#footer {
  position: relative;
  height: 117px;
  width: 100%;
  background-color: rgb(48, 48, 48);
}

#footer li {
  list-style-type: none;
  display: inline-block;
  margin-right: 20px;
}

.row {
  height: 117px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.col-1 {
  height: 100%;
  width: calc(100% / 2);
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

.col-2 {
  height: 100%;
  width: calc(100% / 2);
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

#button {
  color: white;
  padding: 15px 25px;
  background-color: rgb(48, 48, 48);
  border: 2px solid rgb(2, 130, 249);
}

.txtb {
  color: rgb(2, 130, 249);
  font-size: 25px;
  font-weight: 600;
  margin-right: 30px;
}
</style>