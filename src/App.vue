<template>
  <v-app>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<style>
@font-face {
  font-family: "Lalezar";
  src: url("@/assets/Fonts/Lalezar-Regular.ttf");
}
html {
  background-color: #21263d;
}
html,
[class*="text"],
button {
  font-family: "Lalezar", "Roboto" !important;
}
.v-btn {
  letter-spacing: normal !important;
}
</style>

<script setup>
function getImageUrl(iconFilename) {
  // This path must be correct for your file
  return new URL(`../assets/icons/${iconFilename}`, import.meta.url);
}
</script>
