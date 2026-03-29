<template>
  <div>
    <Team />
    <Barista />
  </div>
</template>

<script>
import Barista from "../employee-section/barista.vue";
import Team from "../employee-section/team.vue";

export default {
  components: {
    Team,
    Barista,
  },
};
</script>

<style scoped></style>
