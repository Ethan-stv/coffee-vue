<template>
  <div class="mainDiv">
    <div class="firstDiv">
      <ul class="menu">
        <li>Home</li>
        <li>About</li>
        <li>Menu</li>
        <li>Contact</li>
      </ul>
      <img src="../../assets/images/earlys.svg" alt="Logo" />
      <ul class="cart">
        <li>cart</li>
        <li>search</li>
      </ul>
    </div>
    <div class="secondDiv">
      <span><p></p></span>
      <img src="../../assets/images/star.svg" alt="" />
    </div>
  </div>
</template>

<script></script>

<style scoped>
.firstDiv {
  display: flex;
  height: 15vh;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  padding-right: 10px;
}
.mainDiv {
  display: flex;
  align-items: stretch;
  justify-content: space-between;
  border: 1px black solid;
}
.menu {
  display: flex;
  gap: 20px;
  list-style-type: none;
  font-family: "Space Mono", monospace;
}
.menu li {
  position: relative;
  padding: 5px 0;
  cursor: pointer;
}
.menu li::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: 0;
  width: 0;
  height: 2px;
  background-color: black;
  transition: width 0.3s;
}
.menu li:hover::after {
  width: 100%;
}
.cart {
  display: flex;
  gap: 20px;
  list-style-type: none;
  font-family: "Space Mono", monospace;
  padding-right: 5px;
}
.cart li {
  position: relative;
  padding: 5px 0;
  cursor: pointer;
}

.cart li::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: 0;
  width: 0;
  height: 2px;
  background-color: black;
  transition: width 0.3s;
}

.cart li:hover::after {
  width: 100%;
}
.secondDiv {
  display: flex;
  padding-right: 10px;
  justify-content: center;
  align-items: center;
  gap: 10px;
}
span {
  display: block;
  width: 1px;
  background-color: black;
  align-self: stretch;
}
</style>
