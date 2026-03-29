<template>
  <div class="mainDiv">
    <div class="firstDiv">
      <span class="chicken">
        <img
          src="../../assets/images/chicken.svg"
          alt="chicken"
          class="img"
          width="90px"
        />
      </span>
      <span class="text">
        <h3>EARLY BIRDS</h3>
        <p>Weteringstraat 48,1017 SP</p>
        <p>Amsterdam</p>
        <p>Tel:020-7718364</p>
      </span>
    </div>
    <div class="secondDiv">
      <span>
        <p>My Account</p>
        <p>Checkout</p>
        <p>Cart</p>
        <p>Shop</p>
      </span>
    </div>
    <div class="thirdDiv">
      <span>
        <p>Facebook</p>
        <p>Instagram</p>
        <p>Twitter</p>
      </span>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.mainDiv {
  display: flex;
}
.firstDiv {
  display: flex;
  gap: 30px;
  justify-content: flex-start;
  padding-left: 50px;
  align-items: center;
  padding-top: 30px;
  padding-bottom: 30px;
  width: 600px;
}
.firstDiv h3 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 25px;
}
.secondDiv {
  width: 300px;
  padding-top: 30px;
}
.secondDiv span {
  display: flex;
  flex-direction: column;
  gap: 8px;
  font-family: "Space Mono", monospace;
  font-size: 14px;
}
.thirdDiv {
  padding-top: 30px;
}
.thirdDiv span {
  display: flex;
  flex-direction: column;
  gap: 8px;
  font-family: "Space Mono", monospace;
  font-size: 14px;
}
p,
h3 {
  margin: 0px;
  padding: 0px;
}
.text {
  display: flex;
  flex-direction: column;
  gap: 8px;
}
.text p {
  font-family: "Space Mono", monospace;
  font-size: 10px;
}
</style>
