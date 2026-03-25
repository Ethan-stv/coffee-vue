<template>
  <div class="mainDiv">
    <span class="firstSpan">
      <h3>THE COFFEE THAT'S RIGHT FOR YOU</h3>
    </span>
    <div class="products-row">
      <div
        class="product"
        v-for="(item, index) in products"
        :key="item.id"
        :class="{ 'sold-out': index === products.length - 1 }"
      >
        <img :src="item.image" class="product-img" />
        <span class="info-span">
          <p class="product-name">{{ item.name }}</p>
          <p class="product-price">${{ item.price.toFixed(2) }}</p>
        </span>
      </div>
    </div>
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
.mainDiv {
  display: flex;
  flex-direction: column;
  border-top: 1px black solid;
}
.firstSpan {
  margin-left: 20px;
  display: block;
}
.firstSpan h3 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 40px;
}
.product {
  display: flex;
  flex-direction: column;
  border-left: 1px black solid;
  position: relative;
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
.products-row {
  display: flex;
  justify-content: center;
  flex-direction: row;
  flex-wrap: wrap;
  border: 1px black solid;
}
.product:first-child {
  border-left: none;
}
.info-span {
  padding-left: 15px;
}
.sold-out::after {
  content: "SOLD OUT";
  position: absolute;
  top: 15px;
  right: 0;
  background: black;
  color: white;
  padding: 6px 12px;
  font-size: 12px;
  font-family: "Space Mono", monospace;
  letter-spacing: 1px;
  margin: 0;
}
</style>
