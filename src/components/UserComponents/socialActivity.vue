<template>
  <v-container>
    <v-row>
      <v-col v-for="card in cards" :key="card.text" :cols="12" class="px-0">
        <v-card class="rounded-xxlg " color="#21263d">
          <v-img
            :src="card.src"
            class="align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            cover
          >
          </v-img>
          <v-card-subtitle class="text-left mt-5">
            {{ card.comment }}
            <v-btn
              color="white"
              icon="mdi-comment-outline"
              size="small"
              flat
              variant="text"
            ></v-btn>
            {{ card.Like }}
            <v-btn
              color="white"
              icon="mdi-thumb-up-outline"
              size="small"
              variant="text"
            ></v-btn>
          </v-card-subtitle>
          <v-card-text v-text="card.text"></v-card-text>
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
        text: "بازی کردن برای من بیش از یک سرگرمی است؛ این یک ماجراجویی بی‌پایان در جهان‌های مجازی است. ",
        Like: 10,
        comment: 5,
        src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
      },
      {
        text: "بازی کردن برای من بیش از یک سرگرمی است؛ این یک ماجراجویی بی‌پایان در جهان‌های مجازی است. ",
        Like: 10,
        comment: 8,
      },
    ],
  }),
};
</script>
