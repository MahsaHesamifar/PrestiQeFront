<template>
  <v-container class="container roundBottom">
    <v-row align="center">
      <v-col>{{ UserName }}</v-col>
      <v-col>
        <v-row justify="end">
          <v-icon
            class="logo pa-4 mx-2"
            color="red"
            icon="mdi-youtube"
          ></v-icon>
          <v-icon
            class="logo pa-4 mx-2"
            color="#FD4CE1"
            icon="mdi-instagram"
          ></v-icon>
          <v-icon
            class="logo pa-4 mx-2"
            color="info"
            icon="mdi-twitter"
          ></v-icon>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<style>
.logo {
  background-color: #282f49; /*to do*/
}
.roundBottom {
  border-radius: 0 0 24px 24px;
}
@media only screen and (min-width: 960px) {
  .roundBottom {
    border-radius: 0 12px 12px 12px;
  }
}
</style>

<script>
export default {
  props: {
    UserName: {
      type: String,
      default: "UserName",
    },
    Social: {
      type: Object,
      default: {
        youtube: "https://google.com",
        twitter: "https://google.com",
        instagram: "https://google.com",
      },
    },
  },
};
</script>
