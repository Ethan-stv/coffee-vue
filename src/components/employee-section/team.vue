<template>
  <div class="mainDiv">
    <span class="firstSpan">
      <h3>OUR AWESOME TEAM</h3>
    </span>
    <div class="employee-row">
      <div class="employee" v-for="(item, index) in employee" :key="item.id">
        <img :src="item.image" :alt="item.name" class="emp-img" />
        <h4>{{ item.name }}</h4>
        <p>{{ item.role }}</p>
      </div>
    </div>
  </div>
</template>

<script>
import employee from "../../data/employee.json";
export default {
  data() {
    return {
      employee,
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
.employee-row {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  border-top: 1px black solid;
  border-bottom: 1px black solid;
  padding-left: 20px;
  padding-right: 20px;
}
.employee {
  display: flex;
  flex-direction: column;
  border-left: 1px black solid;
  padding-left: 15px;
  padding-right: 15px;
  padding-top: 20px;
  padding-bottom: 10px;
}
.employee:first-child {
    border-left: none;
}
.emp-img {
  width: 200px;
}
.employee h4 {
  margin: 10px 0 10px 0;
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  font-size: 20px;
}

.employee p {
  margin: 0;
  font-family: "Space Mono", monospace;
  font-size: 15px;
}
</style>
