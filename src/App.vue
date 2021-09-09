<template>
  <div id="app">
    <BlackLines />
    <Header />
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
export default {
  name: "App",
  components: {
    Header,
    Content,
    NavBar,
    Jumbotron,
    Footer,
    BlackLines,
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
