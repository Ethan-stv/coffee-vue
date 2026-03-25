<template>
  <div class="mainDiv">
    <div class="firstDiv">
      <h3>
        SWING BY OUR PLACE<br />
        WE ALSO HAVE FOOD
      </h3>
      <span class="spanImg">
        <img src="../../assets/images/nut.svg" alt="" width="300" />
      </span>
    </div>

    <div class="secondDiv">
      <span>
        <h3>DELIVERY</h3>
        <p>
          Vivamus hendrerit at sapien<br />
          nec mattis. Quisque quis arcu
        </p>
      </span>

      <span>
        <h3>WHOLESALE</h3>
        <p>
          Pellentesque in tempor lorem,<br />
          vel porttitor est.
        </p>
      </span>

      <span>
        <h3>CONSISTENCY</h3>
        <p>
          Aliquam ut arcu sodales,<br />
          gravida quam vitae.
        </p>
      </span>

      <span>
        <h3>QUALITY</h3>
        <p>
          Nam at sapien ligula.<br />
          Morbi maximus scelerisque mi sed.
        </p>
      </span>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.mainDiv {
  display: flex;
  background-color: #fdf1d9;
  height: 100vh;
}

.firstDiv {
  width: 40%;
  display: flex;
  flex-direction: column;
  padding-left: 30px;
  justify-content: space-between;
  border-right: 1px black solid;
  border-bottom: 1px black solid;
}

.firstDiv h3 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 50px;
}

.spanImg {
  display: flex;
  padding-bottom: 30px;
}

.secondDiv {
  width: 60%;
  display: flex;
  flex-direction: column;
  gap: 20px;
  border-bottom: 1px black solid;
}

.secondDiv span {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 20px;
  padding-top: 20px;
  padding-left: 30px;
  border-top: 1px black solid;
}

.secondDiv span:first-child {
  border-top: none;
}

.secondDiv span h3,
.secondDiv span p {
  margin: 0;
}

.secondDiv span h3 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 30px;
}

.secondDiv span p {
  font-family: "Space Mono", monospace;
  font-size: 16px;
}
</style>
