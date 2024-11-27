<template>
  <div class="wrapper">
    <div class="title">
      <h3>
        <slot name="company" />
      </h3>
      <h3>
        <slot name="date" />
      </h3>
    </div>

    <slot />
  </div>
</template>

<style scoped>
.wrapper {
  margin-top: 20px;
}

.title {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-right: 5%;
}

h3 {
  font-weight: 600;
}

@media (max-width: 1024px) {
  .title {
    flex-direction: column;
    align-items: flex-start;
    margin-bottom: 12px;
  }
}
</style>
