<template>
  <v-container>
    <v-row>
      <v-col :cols="12" class="px-0">
        <v-card class="text-center rounded-lg">
          <v-img
            aspect-ratio="1"
            src="@/assets/ProfileAssets/battle pass.png"
            cover
            style="max-height: 16vh"
          >
            <v-card-title
              class="text-white text-center text-h2 pt-4 pb-3"
              style="background-color: rgba(0, 0, 0, 0.3); line-height: 0.5"
              v-text="battlePassData.level"
            ></v-card-title>
            <v-card-text
              class="text-white text-center text-h6"
              style="background-color: rgba(0, 0, 0, 0.3); line-height: 0.5"
              v-text="battlePassData.title"
            >
            </v-card-text>
          </v-img>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  props: {
    battlePassData: {
      type: Object,
      default: {
        level: 8,
        title: "Battle Pass",
        src: "@/assets/ProfileAssets/battle pass.png",
      },
    },
  },
};
</script>
