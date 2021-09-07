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
import Header from "@/components/Header.vue";
import Content from "@/components/Content.vue";
import NavBar from "@/components/NavBar.vue";
import Jumbotron from "@/components/Jumbotron.vue";
import Footer from "@/components/Footer.vue";
import BlackLines from "@/components/BlackLines.vue";
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
    BlackLines

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-size: 13px;
}

.text-white {
  color: white;
}

img {
  max-height: 100%;
}

#app {
  height: 100vh;
  width: 100%;
  font-family: sans-serif;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

ul,
li {
  list-style-type: none;
  text-decoration: none;
}
</style>
