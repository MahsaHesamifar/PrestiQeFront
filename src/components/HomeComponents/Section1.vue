<template>
  <v-row justify="center" class="section1">
    <div class="content">
      <div class="description">
        <div class="text-h2 mb-10">مهم نیست به چه نوع بازی علاقه داری!</div>
        <div class="text-h4 verticalScroll">
          <div class="scrollContnet">
            <div class="my-10 text-purple">برد گیم؟</div>
            <div class="my-10 text-pink">بازی های ویدیویی؟</div>
            <div class="my-10 text-yellow">نقش آفرینی؟</div>
            <div class="my-10 text-yellow">اتاق فرار؟</div>
          </div>
        </div>
        <div class="text-h4 mt-10">"اینجا برا همه جا هست"</div>
      </div>
      <div class="vector">
        <v-img
          src="@/assets/HomeAssets/section1/hands.png"
          class="hands position-relative"
        >
          <v-img
            src="@/assets/HomeAssets/section1/dice1.png"
            class="dice1 position-absolute"
          ></v-img>
          <v-img
            src="@/assets/HomeAssets/section1/dice2.png"
            class="dice2 position-absolute"
          ></v-img>
          <v-img
            src="@/assets/HomeAssets/section1/card1.png"
            class="card1 position-absolute"
          ></v-img>
          <v-img
            src="@/assets/HomeAssets/section1/card2.png"
            class="card2 position-absolute"
          ></v-img>
          <v-img
            src="@/assets/HomeAssets/section1/game.png"
            class="game position-absolute"
          ></v-img>
          <v-img
            src="@/assets/HomeAssets/section1/dice3.png"
            class="dice3 position-absolute"
          ></v-img>
        </v-img>
      </div>
    </div>
  </v-row>
</template>

<style>
@keyframes scrollContnet {
  0% {
    margin-top: -40px;
  }
  14% {
    margin-top: -40px;
  }
  28% {
    margin-top: -120px;
  }
  43% {
    margin-top: -120px;
  }
  56% {
    margin-top: -200px;
  }
  70% {
    margin-top: -200px;
  }
  84% {
    margin-top: -280px;
  }
  100% {
    margin-top: -280px;
  }
}

@keyframes dice1 {
  0% {
    transform: scale(1.3);
    rotate: -23.03deg;
  }
  80% {
    rotate: 45deg;
  }
}
@keyframes dice2 {
  0% {
  }
  50% {
    bottom: 27%;
    left: 32%;
  }
}
@keyframes card1 {
  0% {
  }
  50% {
    left: 21%;
    bottom: 35%;
  }
  100% {
    left: 22%;
    bottom: 34%;
    rotate: -10deg;
  }
}
@keyframes card2 {
  0% {
    top: 290px;
    left: 300px;
  }
  50% {
    top: 295px;
    left: 290px;
    rotate: -14deg;
  }
  100% {
    top: 300px;
    left: 285px;
  }
}
@keyframes game {
  0% {
  }
  50% {
    transform: scale(1.1);
    rotate: 5deg;
  }
  100% {
  }
}
@keyframes dice3 {
  0% {
  }
  50% {
    rotate: -14deg;
    transform: scale(0.7);
  }
  100% {
  }
}

.section1 {
  background-image: url("@/assets/HomeAssets/texture.png");
  background-size: 100% 100%;
  width: 100%;
  display: flex;
  justify-content: space-between;
  margin-bottom: 200px;

  .content {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    padding: 5rem;
    background-color: "$vuetify.theme.current.customColor1";
    .description {
      width: 50%;
      .verticalScroll {
        height: 70px;
        overflow: hidden;
        .scrollContnet {
          animation: scrollContnet 8s ease-in-out infinite alternate;
        }
      }
    }
  }

  .vector {
    width: 50%;
    .hands {
      top: 0;
      left: 0;
      height: 100vh;
      width: 100%;
    }
    .dice1 {
      bottom: 100px;
      left: 45%;
      width: 50px;
      animation: dice1 3s ease-in-out 1ms infinite alternate;
    }
    .dice2 {
      bottom: 30%;
      left: 30%;
      width: 60px;
      animation: dice2 3s ease-in-out 1ms infinite alternate;
    }
    .card1 {
      bottom: 36%;
      left: 20%;
      width: 134px;
      animation: card1 3s ease-in-out 1ms infinite alternate;
    }
    .card2 {
      width: 130px;
      animation: card2 3s ease-in-out 1ms infinite alternate;
    }
    .game {
      top: 10%;
      left: 95px;
      width: 314px;
      animation: game 3s ease-in-out 1ms infinite alternate;
    }
    .dice3 {
      top: 161px;
      right: 15%;
      width: 110px;
      animation: dice3 3s ease-in-out 1ms infinite alternate;
    }
  }
}
</style>

<script setup>
//
</script>
