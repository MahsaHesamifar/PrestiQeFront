<template>
  <v-container class="pa-0 profileBackground" fluid>
    <v-row justify="center" class="profileBackground pa-0 position-relative">
      <v-col cols="12" md="6" class="pa-0"><AttendancesComponents /> </v-col>
    </v-row>
  </v-container>
</template>

<style>
.profileBackground {
  background-color: #6f7079;
}
</style>

<script setup>
import AttendancesComponents from "@/components/AuthComponents/AttendancesComponents.vue";
</script>
