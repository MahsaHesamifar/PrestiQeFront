<template>
  <v-container fluid class="mainContainer bg-background">
    <Header />
    <Section1 />
    <section2 />
    <v-row class="section"> section </v-row>
  </v-container>
</template>

<style>
.mainContainer {
  .section {
    min-height: 100vh;
  }
}
</style>

<script setup>
import Header from "@/components/HomeComponents/Header.vue";
</script>
