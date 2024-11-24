<script setup lang="ts">
import ListItem from "../ListItem.vue"
import DocumentationIcon from "../icons/IconDocumentation.vue"
</script>

<template>
  <ListItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>About Me</template>

    <p>I'm a Full Stack Developer with 3+ years of experience.</p>
    <p>Specializing in frontend technologies, but aiming to improve backend skills.</p>
  </ListItem>
</template>
