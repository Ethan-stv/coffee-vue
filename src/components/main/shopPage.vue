<template>
  <div>
    <Assortment />
    <FoodPage />
    <ReserveTable />
  </div>
</template>

<script>
import Assortment from "../shop-section/assortment.vue";
import FoodPage from "../shop-section/food-page.vue";
import ReserveTable from "../shop-section/reserve-table.vue";

export default {
  components: {
    Assortment,
    FoodPage,
    ReserveTable,
  },
};
</script>

<style scoped></style>
