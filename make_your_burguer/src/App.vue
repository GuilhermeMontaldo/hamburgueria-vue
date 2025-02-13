<template>
  <div>
    <NavBar :logo="logo_src" :alt="alt_name" />
    <router-view />
    <Footer />
  </div>
</template>

<script>
import Footer from "./components/Footer.vue";
import NavBar from "./components/NavBar.vue";

export default {
  components: {
    NavBar,
    Footer,
  },
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Make Your Burguer",
    };
  },
};
</script>

<style>
* {
  font-family: Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}


.main-container {
  margin: 50px;
  min-height: 250px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>