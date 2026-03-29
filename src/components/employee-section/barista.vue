<template>
  <div class="mainDiv">
    <div class="firstDiv">
      <img src="../../assets/images/barista.svg" alt="barista" />
      <div class="about">
        <span>
          <h1>BARISTA SCHOOLS & CAREERS</h1>
          <p>
            We host courses covering everything<br />
            from simple home brewing techniques<br />
            to advanced latte art to allow you<br />
            to learn the essential life skill of<br />
            how to make truly great coffee.
          </p>
        </span>
        <span>
          <BlackButton>VIEW MORE</BlackButton>
        </span>
      </div>
    </div>
    <div class="secondDiv"></div>
  </div>
</template>

<script>
import BlackButton from "@/ui/black-button.vue";

export default {
  components: {
    BlackButton,
  },
};
</script>

<style scoped>
.mainDiv {
  display: flex;
  background-color: #c5d6d1;
  height: 100vh;
  border-bottom: 1px black solid;
}
.firstDiv {
  display: flex;
  flex: 1.8;
  align-items: center;
  justify-content: flex-start;
  padding-left: 80px;
  background-color: #c5d6d1;
  gap: 30px;
}
.about h1 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
}
.about p {
  font-family: "Space Mono", monospace;
  font-size: 15px;
}
.about {
  padding-left: 30px;
}
.about h1 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  margin: 0 0 10px 0;
}
.about p {
  font-family: "Space Mono", monospace;
  font-size: 15px;
  margin: 0;
}
.about span {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  margin-top: 50px;
  margin-bottom: 50px;
}
.firstDiv img {
  width: 80%;
  max-width: 800px;
}
</style>
