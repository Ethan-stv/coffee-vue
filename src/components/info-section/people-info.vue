<template>
  <div class="mainDiv">
    <div class="firstDiv">
      <div class="stars">
        <span v-for="n in 5" :key="n" class="star">★</span>
      </div>

      <p class="firstText">
        "ANOTHER REASON PEOPLE JUST CAN'T KEEP AWAY FROM<br />
        THEIR LOCAL COFFEE SHOP IS THE QUALITY OF COFFEE<br />
        THAT'S ON OFFER."
      </p>
      <p class="secondText">Henry Monro</p>
    </div>
    <div class="secondDiv">
      <img src="../../assets/images/cup.svg" alt="" />
    </div>
  </div>
</template>

<script></script>

<style scoped>
.mainDiv {
  display: flex;
  height: auto;
}
.firstDiv {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 50%;
}
.firstText {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 30px;
  text-align: center;
}
.secondText {
  font-family: "Space Mono", monospace;
  font-size: medium;
}
.stars {
  display: flex;
  gap: 8px;
  margin-bottom: 16px;
}

.star {
  color: #ffd700;
  font-size: 28px;
}

.secondDiv {
  background-color: aqua;
  width: 50%;
  display: flex;
}
.secondDiv img {
    width: 100%;
    margin: auto;
}
</style>
