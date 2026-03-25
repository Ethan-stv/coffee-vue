<template>
  <div>
    <ul class="list">
      <li>fairtrade</li>
      <li>Organic</li>
      <li>Climate neutral</li>
    </ul>
  </div>
</template>

<script></script>

<style scoped>
div {
  display: flex;
  justify-content: center;
  border: 1px black solid;
}
.list {
  display: flex;
  justify-content: center;
  list-style-type: none;
}
.list li {
  font-family: "Space Mono", monospace;
  font-size: small;
  cursor: pointer;
}
.list li:not(:last-child)::after {
  content: "|";
  margin: 0 10px;
  color: black;
}
</style>
