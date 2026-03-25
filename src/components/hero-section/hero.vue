<template>
  <div class="mainDiv">
    <div class="hero">
      <img
        class="heroimage"
        src="../../assets/images/hero_image.svg"
        alt="Hero Image"
      />
      <span class="left-arrow">
        <img src="../../assets/images/left_arrow.svg" alt="" />
      </span>
    </div>

    <div class="enjoy">
      <div class="textWrapper">
        <img class="eff" src="../../assets/images/eff.svg" alt="" />
        <img class="icon" src="../../assets/images/icon.svg" alt="" />
        <p class="penj">ENJOY<br />LIFE SIP<br />BY SIP</p>
        <img class="love" src="../../assets/images/love.svg" alt="" />
      </div>
      <span class="right-arrow">
        <img src="../../assets/images/right_arrow.svg" alt="" />
      </span>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.mainDiv {
  display: flex;
  width: 100%;
  align-items: stretch;
}

.hero {
  position: relative;
  display: inline-block;
}

.heroimage {
  width: 100%;
  max-width: 700px;
  height: auto;
  display: block;
}

.left-arrow {
  position: absolute;
  top: 50%;
  background-color: #fbed81;
  padding: 5px 10px;
  cursor: pointer;
}

.right-arrow {
  position: absolute;
  right: 0;
  top: 50%;
  transform: translateY(-50%); 
  background-color: #fbed81;
  padding: 5px 10px;
  cursor: pointer;
}

.enjoy {
  position: relative;
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  padding-left: 20px;
  overflow: hidden;
}

.textWrapper {
  position: relative;
  width: 100%;
  max-width: 600px;
  margin-left: 10px;
}

.eff {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 120%;
  height: auto;
  z-index: 0;
  opacity: 0.8;
  pointer-events: none;
}

.penj {
  position: relative;
  z-index: 1;
  font-size: 80px;
  line-height: 1.1;
  color: black;
  margin: 0;
  max-width: 80%;
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
}
.icon {
  position: relative;
  width: 120px;
  left: 150px;
  top: 35px;
}
.love {
  position: relative;
  bottom: 60px;
  left: 20px
}
</style>
