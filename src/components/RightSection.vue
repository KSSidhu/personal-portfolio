<script setup lang="ts">
import ListItem from "./ListItem.vue"
import CommunityIcon from "./icons/IconCommunity.vue"
import SupportIcon from "./icons/IconSupport.vue"
import SkillSection from "./skill-list/SkillSection.vue"
import AboutMeSection from "./about-me/AboutMeSection.vue"
import ExperienceSection from "./experience/ExperienceSection.vue"
import EducationSection from "./education/EducationSection.vue"
</script>

<template>
  <AboutMeSection />

  <SkillSection />

  <ExperienceSection />

  <EducationSection />

  <ListItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Community</template>

    Got stuck? Ask your question on
    <a href="https://chat.vuejs.org" target="_blank" rel="noopener">Vue Land</a>, our
    official Discord server, or
    <a href="https://stackoverflow.com/questions/tagged/vue.js" target="_blank" rel="noopener">StackOverflow</a>. You
    should also subscribe to
    <a href="https://news.vuejs.org" target="_blank" rel="noopener">our mailing list</a>
    and follow the official
    <a href="https://twitter.com/vuejs" target="_blank" rel="noopener">@vuejs</a>
    twitter account for latest news in the Vue world.
  </ListItem>

  <ListItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Support Vue</template>

    As an independent project, Vue relies on community backing for its sustainability. You
    can help us by
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">becoming a sponsor</a>.
  </ListItem>
</template>
