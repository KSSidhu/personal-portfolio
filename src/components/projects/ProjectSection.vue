<script setup lang="ts">
import ListItem from "../ListItem.vue"
import KeyboardIcon from "../icons/IconKeyboard.vue"
import ProjectListItem from "./ProjectListItem.vue";
</script>

<template>
  <ListItem>
    <template #icon>
      <KeyboardIcon />
    </template>
    <template #heading>Projects</template>


    <div class="content">
      <ProjectListItem :technologies="['NextJs', 'React', 'Typescript', 'drizzleORM']"
        link="https://github.com/KSSidhu/dev-finder">
        <template #title>Dev Finder</template>
        <template #description>My take on a tutorial by WebDevCody to build a full-stack app to connect developers to
          work
          on projects collaboratively.</template>
      </ProjectListItem>


      <ProjectListItem :technologies="['React', 'Typescript']" link="https://github.com/KSSidhu/colors-box-v2">
        <template #title>Color Box</template>
        <template #description>A palette building SPA allowing users to build custom palettes for their
          projects.</template>
      </ProjectListItem>
    </div>
  </ListItem>
</template>

<style scoped>
.content {
  margin-top: 12px;
  display: flex;
  flex-direction: column;
  gap: 30px;
}
</style>
