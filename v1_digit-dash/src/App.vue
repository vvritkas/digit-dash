<template>
  <Navbar />
  <RouterView />
  <Footer />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";

export default { components: { Navbar, Footer } };
</script>

<style scoped>
#mainWrapper {
  max-width: 1200px;
  margin: 10px auto;
}
</style>
