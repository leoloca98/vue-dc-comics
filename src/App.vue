<template>
  <div id="app">
    <BlackLines />
    <Header />
    <TopJumbotron />
    <Content />
    <Nav-Bar />
    <Jumbotron />
    <Footer />
    <BlackLines />
  </div>
</template>

<script>
import Header from "../src/components/Header.vue";
import Content from "../src/components/Content.vue";
import NavBar from "../src/components/NavBar.vue";
import Jumbotron from "../src/components/Jumbotron.vue";
import Footer from "../src/components/Footer.vue";
import BlackLines from "../src/components/BlackLines.vue";
import TopJumbotron from "../src/components/TopJumbotron.vue";
export default {
  name: "App",
  components: {
    Header,
    Content,
    NavBar,
    Jumbotron,
    Footer,
    BlackLines,
    TopJumbotron,
  },
};
</script>

<style lang="scss">
#app {
  height: 100vh;
  width: 100%;
  font-family: sans-serif;
}

@import "../src/assets/scss/style.scss";
</style>
