<template>
  <div class="mainDiv">
    <div class="navigateDiv">
      <p>LISBON COFFEE SALON</p>
      <p>BERLIN COFFEE ROASTERY</p>
      <p>AMSTERDAM COFFEE SHOP</p>
    </div>
    <div class="guide-img">
      <img
        src="../../assets/images/guide.svg"
        alt="guide"
        width="700"
        height="700"
      />
      <div class="info-img">
        <h3>AMSTERDAM CENTRE COFFEE</h3>
        <span class="span1">
          <p>Weteringstraat 48,1017,Amsterdam</p>
          <p>Tel:020-7718364</p>
          <p>Email:earlybirds@info.com</p>
        </span>
        <span class="span2">
          <p>Mon-Fri..........6.45am-3.00pm</p>
          <p>Sat-Sun.........8.30am-4.00pm</p>
        </span>
        <span>
          <BlackButton>CONTACT US</BlackButton>
        </span>
      </div>
    </div>
  </div>
</template>

<script>
import BlackButton from '@/ui/black-button.vue';

export default {
  components: {
    BlackButton
  },
};
</script>

<style scoped>
.mainDiv {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  height: 100vh;
  background-color: #f8f8f8;
}

.navigateDiv {
  display: flex;
  flex-direction: column;
  writing-mode: vertical-rl;
  transform: rotate(180deg);
  height: 100vh;
  gap: 30px;
  border: 1px black solid;
}

.navigateDiv p {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 50px;
  border-right: 1px black solid;
  display: flex;
  margin: 0px;
  padding: 10px;
  align-items: center;
  box-sizing: border-box;
  text-align: center;
  width: 100px;
}

.navigateDiv p:first-child {
  border-right: none;
}

.guide-img {
  display: flex;
  align-items: flex-start;
  margin-left: 50px;
}
.info-img {
  margin-left: 20px;
  margin-top: 100px;
}
h3 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: 25px;
}
.span1 {
  display: block;
  flex-direction: column;
  margin-bottom: 30px;
}
.span1 p {
  font-family: "Space Mono", monospace;
  font-size: 14px;
}
.span2 {
  display: block;
  margin-bottom: 30px;
}
.span2 p {
  font-family: "Space Mono", monospace;
  font-size: 14px;
}
</style>
