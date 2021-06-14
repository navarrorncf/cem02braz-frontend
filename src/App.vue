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

p.text {
  font-size: 1.7rem;
  max-width: 30em;
  line-height: 1.5;
  margin-bottom: 2em;
  font-variation-settings: "wght" 450;
}
</style>
