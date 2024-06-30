<template>
  <v-container class="pa-0 overflow-hidden" fluid>
    <v-row class="mainBackGroundImage overflow-hidden">
      <v-col cols="12" class="overflow-hidden">
        <v-img
          src="@/assets/AuthAssets/luna 1.png"
          class="luna position-absolute"
        ></v-img>
        <v-img
          src="@/assets/AuthAssets/manny 1.png"
          class="manny position-absolute"
        ></v-img>
        <v-img
          src="@/assets/AuthAssets/Untitled121 1.png"
          class="thunder position-absolute"
        ></v-img>
        <v-img
          src="@/assets/AuthAssets/jax 1.png"
          class="jax position-absolute"
        ></v-img>
      </v-col>
    </v-row>
  </v-container>
</template>

<style>
@keyframes thunderMove {
  0% {
    transform:rotateY(180deg) scale(0.8) rotate(0deg);
  }
  20% {
    transform:rotateY(180deg) scale(0.8)   rotate(-2deg);
  }
  80% {
    transform:rotateY(180deg) scale(0.8)  rotate(15deg);
  }
  100% {
    transform:rotateY(180deg) scale(0.8)  rotate(13deg);
  }
}

@keyframes jaxMove {
  0% {
    bottom: 58%;
  }
  20% {
    bottom: 60%;
  }
  80% {
    bottom: 50%;
  }
  100% {
    bottom: 52%;
  }
}

.mainBackGroundImage {
  background-image: url("@/assets/AuthAssets/bg 1.png");
  background-size: 100% 55%;
  height: 200vh;
}
.jax {
  left: 55vw;
  width: 45vw;
  animation: jaxMove 5s ease-in-out 1ms infinite alternate;
}
.thunder {
  left: 45vw;
  width: 150%;
  bottom: 35%;
  transform-origin: 30% 65%;
  animation: thunderMove 5s ease-in-out 1ms infinite alternate;
}
.luna {
  left: 50vw;
  width: 45vw;
  bottom: 40%;
}
.manny {
  right: 30.2vw;
  width: 20vw;
  bottom: 40%;
}
</style>
