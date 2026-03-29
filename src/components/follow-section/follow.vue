<template>
  <div class="mainDiv">
    <span class="firstSpan">
      <h3>FOLLOW US FOR MORE</h3>
    </span>
    <div class="images">
      <div v-for="(icon, index) in icons" :key="index" class="icon">
        <img :src="icon" alt="icon" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      icons: [
        "/follow1.svg",
        "/follow2.svg",
        "/follow3.svg",
        "/follow4.svg",
        "/follow5.svg",
        "/follow6.svg",
        "/follow7.svg",
        "/follow8.svg",
        "/follow9.svg",
        "/follow10.svg",
      ],
    };
  },
};
</script>

<style scoped>
.mainDiv {
  display: flex;
  flex-direction: column;
  gap: 20px;
  padding-bottom: 20px;
  border-bottom: 1px black solid;
}
.firstSpan {
  border-bottom: 1px solid black;
}
.firstSpan h3 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 40px;
  margin-left: 20px;
}
.images {
  display: flex;
  flex-wrap: wrap;
  margin-left: 20px;
  margin-right: 20px;
  padding-top: 20px;
  gap: 10px;
  justify-content: center;
}
.icon {
  flex: 0 0 calc((100% - 4 * 10px) / 5);
  display: flex;
  justify-content: center;
  margin-bottom: 10px;
}
.icon img {
  width: 100%;
  height: auto;
  object-fit: cover;
}
</style>
