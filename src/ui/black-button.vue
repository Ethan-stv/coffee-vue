<template>
  <button class="base-btn">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "BaseButton",
};
</script>

<style scoped>
.base-btn {
  display: inline;
  background-color: #1d1d1b;
  padding: 15px;
  color: white;
  font-family: "Space Mono", monospace;
  border: 0px;
  cursor: pointer;
  background-image: url("@/assets/images/vector.svg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
}
</style>
