<template>
  <router-view />
</template>

<style>
@font-face {
  font-family: "Montserrat";
  src: url("./assets/fonts/Montserrat-VF.woff2");
}

html {
  font-size: 62.5%;
  scroll-behavior: smooth;
}

body {
  box-sizing: border-box;
  font-size: 1.6rem;
  font-family: "Montserrat", Arial, Helvetica, sans-serif;
  font-variation-settings: "wght" 400;
}

*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}
</style>
