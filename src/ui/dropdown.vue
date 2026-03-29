<template>
  <div class="dropdown" @click="toggle">
    <div class="dropdown-selected">
      {{ modelValue }}
      <span class="arrow" :class="{ open: isOpen }">⌄</span>
    </div>

    <div v-if="isOpen" class="dropdown-menu">
      <div
        v-for="option in options"
        :key="option"
        class="dropdown-item"
        @click.stop="select(option)"
      >
        {{ option }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CustomDropdown",
  props: {
    options: {
      type: Array,
      required: true,
    },
    modelValue: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    toggle() {
      this.isOpen = !this.isOpen;
    },
    select(option) {
      this.$emit("update:modelValue", option);
      this.isOpen = false;
    },
  },
};
</script>

<style scoped>
.dropdown {
  width: 250px;
  cursor: pointer;
  position: relative;
  font-family: "Space Mono", monospace;
}

.dropdown-selected {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 0;
  border-bottom: 2px solid black;
}

.arrow {
  transition: transform 0.3s;
}

.arrow.open {
  transform: rotate(180deg);
}

.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  width: 100%;
  background: white;
  border: 1px solid black;
  margin-top: 5px;
  z-index: 10;
}

.dropdown-item {
  padding: 10px;
}

.dropdown-item:hover {
  background: #f0f0f0;
}
</style>
