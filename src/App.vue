<template>
  <div class="App">
    <Header />
    <MainView />
    <Footer />
  </div>
</template>

<script>
  import MainView from "./views/MainView/MainView.vue";
  import Header from "./components/Header/Header.vue";
  import Footer from "./components/Footer/Footer.vue";

  export default {
    components: {
      Header,
      MainView,
      Footer
    }
  }
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Russo+One&display=swap");
*,
:after,
:before {
  box-sizing: border-box;
}

body,
html {
  margin: 0;
  padding: 0;
  font-family: "Montserrat", sans-serif;
  background-color: #0e0e18;
  color: #dbdbdc;
  line-height: 1.5;
}

.bat {
  font-family: 'Russo One', sans-serif;
}
</style>
