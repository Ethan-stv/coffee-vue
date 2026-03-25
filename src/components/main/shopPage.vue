<template>
  <div>
    <Assortment />
    <FoodPage />
  </div>
</template>

<script>
import Assortment from "../shop-section/assortment.vue";
import FoodPage from "../shop-section/food-page.vue";

export default {
  components: {
    Assortment,
    FoodPage,
  },
};
</script>

<style scoped></style>
