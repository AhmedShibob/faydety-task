<template>
  <div id="app">
    <Navber />
    <Home />
    <Footer />
  </div>
</template>

<script>
import Home from "./pages/home/index";
import Footer from "./components/footer/footer";
import Navber from "./components/navber/navber";

export default {
  name: "App",
  components: {
    Home,
    Navber,
    Footer
  },
};
</script>


