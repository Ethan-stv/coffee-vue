<template>
  <HeaderPage />
  <InfoPage />
  <ShopPage />
</template>

<script>
import HeaderPage from "./components/main/headerPage.vue";
import InfoPage from "./components/main/infoPage.vue";
import ShopPage from "./components/main/shopPage.vue";

export default {
  components: {
    HeaderPage,
    InfoPage,
    ShopPage,
  },
};
</script>

<style scoped></style>
