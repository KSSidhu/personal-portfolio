<script setup lang="ts">
import { computed } from "vue";

const { color } = defineProps<{ color: "blue" | "red" | "green" | "purple" }>()


const classObject = computed(() => ({
  blue: color === "blue",
  green: color === "green",
  purple: color === "purple",
  red: color === "red",
}))
</script>

<template>
  <span :class="classObject">
    <slot />
  </span>
</template>

<style scoped>
span {
  border-radius: 20px;
  padding: 4px 8px;
  font-weight: 500;
  display: flex;
  align-items: center;
}

.blue {
  color: rgb(59 130 246);
  background-color: #1D3356;
}

.red {
  color: rgb(239 68 68);
  background-color: #542020;
}

.green {
  color: rgb(34 197 94);
  background-color: #164828;
}

.purple {
  color: rgb(168 85 247);
  background-color: #3F2557;
}
</style>
