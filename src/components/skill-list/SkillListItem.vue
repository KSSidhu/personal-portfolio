<script setup lang="ts">
import SkillTag from "./SkillTag.vue"
const { title, items, color } = defineProps<{
  title: string, items: string[],
  color: "blue" | "red" | "green" | "purple"
}>()

</script>

<template>
  <div>
    <h2>{{ title }}</h2>

    <div class="tags">
      <template v-for="item in items" v-bind:key="item">
        <SkillTag :color="color">{{ item }}</SkillTag>
      </template>
    </div>
  </div>
</template>

<style scoped>
.tags {
  display: flex;
  gap: 8px;
}

h2 {
  font-weight: 400;
}
</style>
