<template>
  <HeaderPage />
  <InfoPage />
  <ShopPage />
  <EmployeePage />
  <SuppliesPage />
  <FollowPage />
  <Footer />
</template>

<script>
import Footer from "./components/footer/footer.vue";
import EmployeePage from "./components/main/employeePage.vue";
import FollowPage from "./components/main/followPage.vue";
import HeaderPage from "./components/main/headerPage.vue";
import InfoPage from "./components/main/infoPage.vue";
import ShopPage from "./components/main/shopPage.vue";
import SuppliesPage from "./components/main/suppliesPage.vue";

export default {
  components: {
    HeaderPage,
    InfoPage,
    ShopPage,
    EmployeePage,
    SuppliesPage,
    FollowPage,
    Footer,
  },
};
</script>

<style scoped></style>
