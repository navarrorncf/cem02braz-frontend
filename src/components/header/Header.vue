<template>
  <header class="hero-header">
    <NavigationMenu />
    <HeaderContent />
  </header>
</template>

<script>
import NavigationMenu from "./NavigationMenu.vue";
import HeaderContent from "./HeaderContent.vue";

export default {
  name: "Header",
  components: {
    NavigationMenu,
    HeaderContent,
  },
};
</script>

<style>
header.hero-header {
  height: 100vh;
  width: 100vw;
  background: linear-gradient(to left, #f1eade88, #f1eade88),
    url("../../assets/images/books.jpg") center center / cover;
  overflow: hidden;
}
</style>
