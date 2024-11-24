<script setup lang="ts">
import ListItem from "../ListItem.vue"
import ToolingIcon from "../icons/IconTooling.vue"
import LanguageSection from "./LanguageSection.vue"
import FrameworkSection from "./FrameworkSection.vue"
import BackendSection from "./BackendSection.vue"
import DatabaseSection from "./DatabaseSection.vue"
</script>

<template>
  <ListItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Skills</template>

    <div class="sections">
      <LanguageSection />

      <FrameworkSection />

      <BackendSection />

      <DatabaseSection />
    </div>
  </ListItem>
</template>

<style scoped>
.sections {
  display: flex;
  gap: 12px;
  flex-direction: column;
}
</style>
