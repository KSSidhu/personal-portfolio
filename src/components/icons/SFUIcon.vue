<script setup lang="ts">
import SFUIcon from "../../assets/SFU_block_colour_cmyk.svg"
</script>
<template>
  <div>
    <img :src="SFUIcon" />
  </div>
</template>

<style scoped>
div {
  background-color: var(--vt-c-white);
  padding: 12px;
  border-radius: 50%;
}

img {
  height: 80px;
  width: 80px;
}
</style>
