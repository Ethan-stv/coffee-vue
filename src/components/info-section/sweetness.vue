<template>
  <div>
    <span class="firstSpan">
      <span>
        <p class="firstText">
          OUR BLENDS DELIVER ON THE PROMISE OF<br />
          BALANCE AND CONSISTENCY, ROASTED TO<br />
          MAXIMIZE SWEETNESS.
        </p>
        <p class="secondText">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut <br />
          elit tellus, luctus nec ullamcorper
        </p>
      </span>
      <span class="view-more">
        <router-link>VIEW MORE</router-link>
        <img src="../../assets/images/right_arrow.svg" width="20px" />
      </span>
    </span>
    <span class="secondSpan">
      <div class="product" v-for="item in products.slice(0, 2)" :key="item.id">
        <img :src="item.image" class="product-img" />
        <span class="info-span">
          <p class="product-name">{{ item.name }}</p>
          <p class="product-price">${{ item.price.toFixed(2) }}</p>
        </span>
      </div>
    </span>
  </div>
</template>

<script>
import products from "../../data/products.json";
export default {
  data() {
    return {
      products,
    };
  },
};
</script>

<style scoped>
div {
  display: flex;
  height: 500px;
  background-color: #fdf1d9;
  justify-content: space-between;
  border: 0.5px black solid;
}
.firstSpan {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin-left: 100px;
  padding-top: 40px;
  padding-bottom: 40px;
}
.firstText {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 35px;
}
.secondText {
  font-family: "Space Mono", monospace;
  font-size: 16px;
}
router-link {
  font-family: "Space Mono", monospace;
  font-weight: bold;
  cursor: pointer;
}
.view-more {
  display: flex;
  gap: 5px;
}
.secondSpan {
  display: flex;
  align-items: center;
}
.product {
  display: flex;
  width: 370px;
  flex-direction: column;
}
.product-img {
  width: 350px;
}
.product-name {
  font-family: "Space Mono", monospace;
  font-weight: bold;
}
.product-price {
  font-family: "Space Mono", monospace;
  color: #6b4f3a;
}
.info-span {
  display: flex;
  flex-direction: column;
  align-self: flex-start;
  gap: 15px;
  margin-left: 20px;
  margin-bottom: 20px;
}
.info-span p {
  margin: 0;
}
</style>
