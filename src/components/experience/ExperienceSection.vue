<script setup lang="ts">
import ListItem from "../ListItem.vue"
import ExperienceListItem from "./ExperienceListItem.vue"
import EcosystemIcon from "../icons/IconEcosystem.vue"
</script>

<template>
  <ListItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Experience</template>

    <ExperienceListItem>
      <template #company>Disco Inc - FullStack Developer</template>
      <template #date>July 2022 - Present</template>

      <ul>
        <li>Developed the foundational work for an initial app release using React Native</li>
        <li>Ported our web content editor to React Native, removing the bottleneck to port our webviews to native code
        </li>
        <li>Building highly interactive, dynamic features using TypeScript, React and Relay on the frontend and Node,
          GraphQL, TypeORM and PostgreSQL on the backend.</li>
      </ul>
    </ExperienceListItem>


    <ExperienceListItem>
      <template #company>Sierra Wireless - Co-op Developer</template>
      <template #date>May 2021 - Dec 2021</template>

      <ul>
        <li>Implemented Douglas-Peucker algorithm to reduce loading time for geoJson data in google maps.</li>
        <li>Implemented new features and fixed bugs improving overall user experience with application.</li>
      </ul>
    </ExperienceListItem>


    <ExperienceListItem>
      <template #company>SAP - Co-op Developer</template>
      <template #date>May 2019 - Dec 2019</template>

      <ul>
        <li>Fixed UI navigation bugs, improving user experience with the software.</li>
        <li>Expanded the team’s Selenium testing framework to cover workflows for existing and new features, reducing
          the
          possibility of UI errors in production.</li>
        <li>Repaired failing Jasmine integration tests for two new features ensuring our team met the feature release
          deadline.</li>
      </ul>
    </ExperienceListItem>
  </ListItem>
</template>
