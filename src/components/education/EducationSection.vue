<script setup lang="ts">
import DocumentationIcon from "../icons/IconDocumentation.vue"
import ListItem from "../ListItem.vue"
import SFUIcon from "../icons/SFUIcon.vue"
</script>

<template>
  <ListItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Education</template>

    <div class="content">
      <SFUIcon />
      <div class="info">
        <h2>Simon Fraser University</h2>
        <h3>Bachelor of Computer Science - Software Systems</h3>
        <p>2018 - 2022</p>
      </div>

    </div>
  </ListItem>
</template>

<style scoped>
.content {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 12px;
  margin-top: 12px;
}

.info {
  display: flex;
  flex-direction: column;
}

h2 {
  font-weight: 600;
}
</style>
