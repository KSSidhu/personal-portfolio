<script setup lang="ts">
import ListItem from "../ListItem.vue"
import ProfileIcon from "../icons/IconProfile.vue"
</script>

<template>
  <ListItem>
    <template #icon>
      <ProfileIcon />
    </template>
    <template #heading>About Me</template>

    <div>
      <p>I'm a Full Stack Developer with 3+ years of experience.</p>
      <p>Specializing in frontend technologies, but aiming to improve backend skills.</p>
    </div>
  </ListItem>
</template>

<style scoped>
div {
  margin-top: 12px;
}
</style>
