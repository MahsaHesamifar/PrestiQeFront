<template>
  <v-container fluid>
    <v-row justify="center" class="profileBackground">
      <v-col cols="12" sm="8" md="7">
        <v-row justify="center">
          <v-col cols="12" md="3"><avatar /></v-col>
          <v-col cols="10" md="9">
            <SocialNetworkStatsVue />
          </v-col>
        </v-row>
        <v-row justify="center" class="my-n6">
          <v-col cols="10" md="12" class="pe-3"> <SocialData /> </v-col
        ></v-row>
        <v-row cols="10" md="12" class="mx-11 mx-md-0"><bio /> </v-row>
        <v-row cols="10" md="12" class="mx-11 mx-md-0" justify="center"
          ><Navigation />
        </v-row>
      </v-col>
      <v-col cols="5" md="2">
        <v-row justify="center">
          <v-col cols="6" md="12"><battlePass /></v-col>
          <v-col cols="5" md="12"><statue /></v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<style>
.profileBackground {
  background-image: url("@/assets/ProfileAssets/VJl.gif");

  background-size: 100% 100%;
}
</style>

<script setup>
import avatar from "@/components/UserComponents/Avatar.vue";
import SocialNetworkStatsVue from "@/components/UserComponents/SocialNetworkStats.vue";
import SocialData from "@/components/UserComponents/Social.vue";
import bio from "@/components/UserComponents/bio.vue";
import Navigation from "@/components/UserComponents/Navigation.vue";
import battlePass from "@/components/UserComponents/battlePass.vue";
import statue from "@/components/UserComponents/statue.vue";
</script>
