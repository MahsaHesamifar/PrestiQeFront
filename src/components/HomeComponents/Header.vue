<template>
  <v-row justify="center" class="container">
    <v-img src="@/assets/HomeAssets/header/bg.png" class="bg"></v-img>
    <v-img
      src="@/assets/HomeAssets/header/klif1.png"
      class="klif1 position-absolute"
    ></v-img>
    <v-img
      src="@/assets/HomeAssets/header/lightning.png"
      class="lightning position-absolute"
    ></v-img>
    <v-img
      src="@/assets/HomeAssets/header/players.png"
      class="players position-absolute"
    ></v-img>
    <v-img
      src="@/assets/HomeAssets/header/klif2.png"
      class="klif2 position-absolute"
    ></v-img>
    <v-img
      src="@/assets/HomeAssets/header/bottomSection.png"
      class="bottomSection position-absolute"
    ></v-img>
    <div class="description position-absolute">
      <div class="text-h4">این جا</div>
      <div class="text-h2">اسم سایته!</div>
      <p class="text-h6">
        پاتوق گیمرهای باهوش، جایی برای رقابت، یادگیری و لذت بردن از بازی‌های
        جذاب!
      </p>
    </div>
    <div class="swipeDown position-absolute">
      <v-icon icon="mdi-arrow-down" class="arrow"></v-icon>
    </div>
  </v-row>
</template>

<style>
@keyframes arrow {
  0% {
    bottom: 10px;
  }
  50% {
  }
  100% {
    bottom: 0;
  }
}
.container {
  position: relative;
  width: 100vw;
  .arrow {
    animation: arrow 0.8s ease-in-out 1ms infinite alternate;
  }
  .bg {
    width: 100vw;
    bottom: 0;
  }
  .klif1 {
    width: 100vw;
    bottom: 0;
  }
  .lightning {
    width: 100vw;
    bottom: 0;
  }
  .players {
    width: 100vw;
    bottom: 0;
  }
  .klif2 {
    width: 100vw;
    bottom: 0;
  }
  .bottomSection {
    width: 100vw;
    bottom: 0;
  }
  .description {
    right: 50vw;
    bottom: 30%;
    width: 35%;
  }
  .swipeDown {
    bottom: 30px;
    background: rgba(255, 255, 255, 0.253);
    backdrop-filter: blur(5px);
    border: 2px white solid;
    border-radius: 24px;
    padding: 20px 10px;
  }
}
</style>

<script setup>
//
</script>
