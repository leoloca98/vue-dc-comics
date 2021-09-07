<template>
  <div id="nav-bar">
    <div class="container">
      <div class="content">
        <div class="logo">
          <img alt="DC Logo" src="@/assets/img/dc-logo.png" />
        </div>
        <div class="menu">
          <ul>
            <li>CHARACTERS</li>
            <li>COMICS</li>
            <li>MOVIES</li>
            <li>TV</li>
            <li>GAMES</li>
            <li>COLLETIBLES</li>
            <li>VIDEOS</li>
            <li>FANS</li>
            <li>NEWS</li>
            <li>SHOP</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
#nav-bar {
  height: 120px;
  width: 100%;
  background-color: white;
}

.content {
  display: flex;
  height: 100%;
  width: 100%;
  justify-content: space-between;
}

.logo {
  height: 100%;
}

.logo img {
  max-height: 90px;
  margin: 15px;
}

.menu {
  height: 100%;
}

ul,
li {
  display: inline-block;
  list-style-type: none;
  line-height: 100px;
  padding-right: 15px;
  font-size: 15px;
}
</style>