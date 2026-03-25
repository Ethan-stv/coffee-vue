<template>
  <main>
    <Sweetness />
    <MoreInfo />
    <PeopleInfo />
    <ContactUs />
  </main>
</template>

<script>
import ContactUs from "../info-section/contact-us.vue";
import MoreInfo from "../info-section/more-info.vue";
import PeopleInfo from "../info-section/people-info.vue";
import Sweetness from "../info-section/sweetness.vue";

export default {
  components: {
    Sweetness,
    MoreInfo,
    PeopleInfo,
    ContactUs,
  },
};
</script>

<style scoped></style>
