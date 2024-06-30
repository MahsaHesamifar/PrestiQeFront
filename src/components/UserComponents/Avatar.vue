<template>
  <div class="d-flex justify-center mx-10 mx-sm-10 mx-md-0 my-2">
    <v-avatar
      class="avatar roundedAvatar rounded-lg"
      image="@/assets/ProfileAssets/avatar.png"
      size="7rem"
    ></v-avatar>
  </div>
</template>

<script>
export default {
  props: {
    urlImage: {
      type: String,
      default: "@/assets/logo.png",
    },
  },
};
</script>

<style>
.avatar {
  border-radius: 2vh;
}
</style>
