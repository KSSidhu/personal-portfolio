<script setup lang="ts">
import GithubMarkIcon from "./icons/GithubMark.vue"
import EmailIcon from "./icons/EmailIcon.vue"
import LinkedInIcon from "./icons/LinkedInIcon.vue"
</script>

<template>
  <header>
    <img alt="Profile" src="../assets/images/profile.JPG" />

    <div>
      <h1>Gurkirat Sidhu</h1>
      <h2>Full Stack Developer</h2>

      <h3>📍 Burnaby, BC, Canada </h3>
    </div>

    <div class="icons">
      <GithubMarkIcon />
      <EmailIcon />
      <LinkedInIcon />
    </div>
  </header>
</template>

<style scoped>
img {
  height: 120px;
  width: 120px;
  border-radius: 50%;
}

header {
  padding: 8%;
  position: fixed;
  left: 0;
  right: 60%;
  top: 0;
  display: flex;
  gap: 8px;
  align-items: flex-start;
  flex-direction: column;
}

.icons {
  display: flex;
  flex-direction: row;
  gap: 8px;
}
</style>
