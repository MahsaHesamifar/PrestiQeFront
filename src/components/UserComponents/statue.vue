<template>
  <v-container>
    <v-row justify="center">
      <v-col cols="12" class="position-relative mx-0 px-0">
        <div
          class="position-absolute childStatueCss"
          style="width: 100%; bottom: 0"
        >
          <v-img src="@/assets/ProfileAssets/hologram2 3.png"></v-img>
        </div>
        <v-img src="@/assets/ProfileAssets/character.png"></v-img>
      </v-col>
    </v-row>
  </v-container>
</template>

<style>
@media only screen and (min-width: 960px) {
  .roundBottom {
    border-radius: 0 12px 12px 12px;
  }
}
</style>
