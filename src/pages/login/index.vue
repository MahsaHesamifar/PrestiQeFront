<template>
  <v-container class="pa-0 profileBackground" fluid>
    <v-row justify="center" class="profileBackground pa-0 position-relative">
      <v-col cols="12" md="6" class="pa-0"><ImagePart /></v-col>
      <v-col cols="12" md="6" class="pa-0"><LoginComponents /> </v-col>
    </v-row>
  </v-container>
</template>

<style>
.profileBackground {
  background-color: #21263d;
}
</style>

<script setup>
import ImagePart from "@/components/AuthComponents/ImagePart.vue";
import LoginComponents from "@/components/AuthComponents/LoginComponents.vue";
</script>
