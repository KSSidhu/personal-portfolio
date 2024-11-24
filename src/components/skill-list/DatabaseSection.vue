<script setup lang="ts">
import SkillListItem from "./SkillListItem.vue"
</script>

<template>
  <SkillListItem title="Databases" :items="['Postgres', 'MySQL', 'MongoDB']" color="red" />
</template>
