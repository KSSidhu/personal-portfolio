<script setup lang="ts">
import SkillTag from '../skill-list/SkillTag.vue';
import GithubMark from '../icons/GithubMark.vue';

const { technologies, link } = defineProps<{
  link: string
  technologies: string[]
}>()
</script>
<template>
  <div>
    <h2>
      <slot name="title" />
    </h2>

    <p>
      <slot name="description" />
    </p>

    <div class="tags">
      <template v-for="technology in technologies" v-bind:key="technology">
        <SkillTag color="blue">{{ technology }}</SkillTag>
      </template>
    </div>

    <a v-bind:href="link" target="_blank">
      <GithubMark />
      <p>View Code</p>
    </a>
  </div>
</template>

<style scoped>
h2 {
  font-weight: 600;
}

div {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

a {
  display: flex;
  flex-direction: row;
  gap: 8px;
  color: white;
  width: fit-content;
  background-color: transparent;
  border-radius: 12px;
}

a:hover {
  color: var(--vt-c-black);
  background-color: var(--vt-c-mint-green)
}

.tags {
  display: flex;
  flex-direction: row;
  gap: 12px;
}
</style>
