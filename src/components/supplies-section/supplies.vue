<template>
  <div class="mainDiv">
    <span class="firstSpan">
      <h3>OUR TRUSTED SUPPLIES</h3>
    </span>

    <div class="icon-row">
      <div v-for="(icon, index) in icons" :key="index" class="icon">
        <img :src="icon" alt="icon" />
      </div>
    </div>

    <div class="coffee-section">
      <div class="our-coffee">
        <div class="menu">
          <div v-for="(item, index) in menu" :key="index" class="menu-item">
            <div class="top-line">
              <div class="title-dots">
                <span class="title">{{ item.title }}</span>
                <span class="dots"></span>
              </div>
              <span class="price">{{ item.price }}</span>
            </div>
            <p class="desc">{{ item.desc }}</p>
          </div>
        </div>
      </div>
      <div class="image">
        <img src="../../assets/images/supp.svg" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      icons: [
        "/icon1.svg",
        "/icon2.svg",
        "/icon3.svg",
        "/icon4.svg",
        "/icon5.svg",
      ],
      menu: [
        { title: "CAFFEE LATTE", desc: "Fresh brewed coffee", price: "5.00$" },
        { title: "CAPPUCINO", desc: "Espresso and milk", price: "7.00$" },
        { title: "ICE COFFEE", desc: "Cold brewed espresso", price: "4.00$" },
        { title: "MOCHA", desc: "Espresso, mocha sauce, milk", price: "7.00$" },
        { title: "ESPRESSO", desc: "Rich espresso with milk", price: "4.00$" },
      ],
    };
  },
};
</script>

<style scoped>
.mainDiv {
  display: flex;
  flex-direction: column;
}
.firstSpan {
  margin-left: 20px;
}
.firstSpan h3 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 40px;
}
.icon-row {
  display: flex;
  justify-content: space-between;
  border-top: 1px solid black;
  border-bottom: 1px solid black;
}
.icon {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  border-left: 1px solid black;
  height: 200px;
}
.icon:first-child {
  border-left: none;
}
.icon img {
  width: 150px;
  height: 60px;
}
.coffee-section {
  display: flex;
  width: 100%;
  border-bottom: 1px black solid;

}
.image {
  width: 50%;
  background-color: #eee;
}
.our-coffee {
  width: 50%;
  padding-top: 80px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.menu {
  width: 80%;
  display: flex;
  flex-direction: column;
}
.menu-item {
  display: flex;
  flex-direction: column;
  padding: 5px 25px;
  gap: 5px;
}
.top-line {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.title {
  white-space: nowrap;
  margin-right: 5px;
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  font-size: 20px;
}
.dots {
  display: inline-block;
  width: 100px;
  border-bottom: 1px dotted black;
  margin-left: 1px;
}
.price {
  white-space: nowrap;
  font-family: "Space Mono", monospace;
}
.desc {
  margin-top: 2px;
  color: #333;
  font-family: "Space Mono", monospace;
  font-size: 15px;
}
.image {
  width: 50%;
  height: 100%;
  overflow: hidden;
  display: flex;
}
.image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
