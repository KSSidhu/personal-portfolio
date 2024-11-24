<script setup lang="ts">
import AboutMeHeader from "./components/AboutMeHeader.vue"
import RightSection from "./components/RightSection.vue"
</script>

<template>
  <main>
    <AboutMeHeader />

    <div class="rightColumn">
      <RightSection />
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


@media (max-width: 1024px) {
  .rightColumn {
    position: relative;
    left: 0;
  }
}
</style>
