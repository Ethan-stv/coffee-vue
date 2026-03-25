<template>
  <header>
    <FreeShipping />
    <Header />
    <Hero />
    <UnderHero />
  </header>
</template>

<script>
import FreeShipping from "../header-section/free-shipping.vue";
import Header from "../header-section/header.vue";
import Hero from "../hero-section/hero.vue";
import UnderHero from "../hero-section/under-hero.vue";

export default {
  components: {
    FreeShipping,
    Header,
    Hero,
    UnderHero,
  },
};
</script>

<style scoped></style>
