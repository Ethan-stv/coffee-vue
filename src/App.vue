<template>
  <HeaderPage />
  <InfoPage />
  <Assortment />
</template>

<script>
import HeaderPage from "./components/main/headerPage.vue";
import InfoPage from "./components/main/infoPage.vue";
import Assortment from "./components/shop-section/assortment.vue";

export default {
  components: {
    HeaderPage,
    InfoPage,
    Assortment
  },
};
</script>

<style scoped></style>
