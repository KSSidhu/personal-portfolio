<script setup lang="ts">
import GithubMarkIcon from "./icons/GithubMark.vue"
import EmailIcon from "./icons/EmailIcon.vue"
import LinkedInIcon from "./icons/LinkedInIcon.vue"
</script>

<template>
  <header>
    <img alt="Profile" src="./profile.jpg" />

    <div>
      <h1>Gurkirat Sidhu</h1>
      <h2>Full Stack Developer</h2>

      <h3>📍 Burnaby, BC, Canada </h3>
    </div>

    <div class="icons">
      <a href="https://github.com/KSSidhu" target="_blank">
        <GithubMarkIcon />
      </a>

      <a href="mailto:kirat.sidhu.sw@gmail.com">
        <EmailIcon />
      </a>

      <a href="https://www.linkedin.com/in/gurkiratsidhu-1805/" target="_blank">
        <LinkedInIcon />
      </a>
    </div>
  </header>
</template>

<style scoped>
img {
  height: 150px;
  width: 150px;
  border-radius: 50%;
}

header {
  padding: 4% 10%;
  position: fixed;
  left: 0;
  right: 60%;
  top: 0;
  display: flex;
  gap: 8px;
  align-items: flex-start;
  flex-direction: column;
}

h1 {
  font-weight: 700;
  font-size: 2.25rem;
}

h2 {
  font-weight: 500;
  color: var(--vt-c-mint-green);
}

a {
  display: flex;
  text-decoration: none;
  align-items: center;
}

a:hover {
  background-color: transparent;
  border-radius: 12px;
}

svg {
  color: rgb(156 163 175);
}

svg:hover {
  color: #fff;
}

.icons {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 8px;
}


@media (max-width: 1024px) {
  header {
    padding: 8%;
    position: relative;
  }
}
</style>
