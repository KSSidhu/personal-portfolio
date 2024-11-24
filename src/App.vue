<script setup lang="ts">
import AboutMe from "./components/AboutMe.vue"
import TheWelcome from "./components/TheWelcome.vue"
</script>

<template>
  <main>
    <AboutMe />

    <div class="rightColumn">
      <TheWelcome />
      <TheWelcome />
    </div>
  </main>
</template>

<style scoped>
main {
  padding: 10%;
}


.rightColumn {
  padding-top: 1rem;
  padding-bottom: 1rem;
  padding-right: 1rem;
  position: absolute;
  top: 0;
  right: 0;
  left: 40%;
}
</style>
