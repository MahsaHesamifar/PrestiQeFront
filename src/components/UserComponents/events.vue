<template>
  <v-container>
    <v-row>
      <v-col v-for="card in cards" :key="card.title" :cols="12" class="px-0">
        <v-card class="rounded-xxlg" :color="card.color">
          <v-card-title v-text="card.title"></v-card-title>
          <v-card-subtitle class="bg-black text-left" opacity="1">
            تا {{ card.timeRemain }}</v-card-subtitle
          >
          <v-img
            :src="card.src"
            class="align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            cover
          >
          </v-img>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<style>
.rounded-xxlg {
  border-radius: 24px;
}
</style>

<script>
export default {
  data: () => ({
    cards: [
      {
        title: "ایونت شماره یک",
        timeRemain: "2 روز دیگر",
        src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
        color: "yellow",
      },
      {
        title: "ایونت شماره دو",
        timeRemain: "8 ساعت 34 دقیقه",
        src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
        color: "blue",
      },
    ],
  }),
};
</script>
