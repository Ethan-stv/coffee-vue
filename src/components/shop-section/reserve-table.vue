<template>
  <div class="mainDiv">
    <h1>RESERVE YOUR TABLE</h1>
    <div class="row">
      <Dropdown v-model="people" :options="peopleOptions" />
      <Dropdown v-model="time" :options="timeOptions" />
      <input type="date" :min="today" />
      <BlackButton>BOOK A TABLE</BlackButton>
    </div>
  </div>
</template>

<script>
import BlackButton from "@/ui/black-button.vue";
import Dropdown from "@/ui/dropdown.vue";

export default {
  components: {
    Dropdown,
    BlackButton,
  },
  data() {
    return {
      people: "1 person",
      time: "11:00",

      peopleOptions: ["1 person", "2 people", "3 people", "4 people"],

      timeOptions: [
        "11:00",
        "12:00",
        "13:00",
        "14:00",
        "15:00",
        "16:00",
        "17:00",
        "18:00",
        "19:00",
        "20:00",
        "21:00",
        "22:00",
      ],
      today: new Date().toISOString().split("T")[0],
    };
  },
};
</script>

<style scoped>
.mainDiv {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 60vh;
  gap: 30px;
  flex-direction: column;
  background-image: url('../../assets/images/eff.svg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
h1 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 50px;
}
.row {
  display: flex;
  gap: 20px;
}

.row > * {
  flex-shrink: 0;
}
</style>
