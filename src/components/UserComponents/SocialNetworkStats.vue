<template>
  <v-container class="container roundTop" justify="center">
    <v-row class="ma-1" justify="space-around">
      <v-col>
        <v-row justify="center">
          <div
            class="number pa-2 text-no-wrap rounded-lg text-h6 text-md-h5 text-lg-h4 text-center"
          >
            {{ Stats.PostNumber }}
          </div>
        </v-row>
        <v-row
          class="text-h6 text-no-wrap text-md-h6 text-lg-h5"
          justify="center"
          >پست</v-row
        >
      </v-col>
      <v-col>
        <v-row justify="center">
          <div
            class="number pa-2 text-no-wrap rounded-lg text-h6 text-md-h5 text-lg-h4 text-center"
          >
            {{ Stats.FollowerNumber }}
          </div>
        </v-row>
        <v-row
          class="text-h6 text-no-wrap text-md-h6 text-lg-h5"
          justify="center"
          >دنبال کننده</v-row
        >
      </v-col>
      <v-col>
        <v-row justify="center">
          <div
            class="number pa-2 text-no-wrap rounded-lg text-h6 text-md-h5 text-lg-h4 text-center"
          >
            {{ Stats.FollowingNumber }}
          </div>
        </v-row>
        <v-row
          class="text-h6 text-no-wrap text-md-h6 text-lg-h5"
          justify="center"
        >
          دنبال می کند
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<style>
.roundTop {
  border-radius: 24px 24px 0 0;
}
@media only screen and (min-width: 960px) {
  .roundTop {
    border-radius: 12px 12px 0 0;
  }
}
.container {
  background-color: #21263d; /*todo */
}
.number {
  background-color: #282f49; /*todo */
}
</style>

<script>
export default {
  props: {
    Stats: {
      type: Object,
      default: {
        PostNumber: 5,
        FollowerNumber: 100,
        FollowingNumber: 15,
      },
    },
  },
};
</script>
