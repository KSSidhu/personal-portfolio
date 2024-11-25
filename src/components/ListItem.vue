<template>
  <div class="item">
    <i>
      <slot name="icon"></slot>
    </i>
    <div class="details">
      <h1>
        <slot name="heading"></slot>
      </h1>
      <slot></slot>
    </div>
  </div>
</template>

<style scoped>
.item {
  margin-top: 2rem;
  display: flex;
  position: relative;
}

.details {
  flex: 1;
  margin-left: 1rem;
}

i {
  display: flex;
  place-items: center;
  place-content: center;
  width: 32px;
  height: 32px;

  color: var(--vt-c-orange);
}

h1 {
  font-weight: 700;
}

h3 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}

@media (min-width: 1024px) {
  .item {
    margin-top: 0;
    padding: 0.4rem 0 1rem calc(var(--section-gap) / 2);
  }

  i {
    top: calc(50% - 25px);
    left: -26px;
    position: absolute;
    border: 1px solid var(--vt-c-mint-green);
    background: var(--color-background);
    border-radius: 8px;
    width: 50px;
    top: 0;
    height: 50px;
    margin-top: 12px;
  }

  .item:before {
    content: " ";
    border-left: 1px solid var(--vt-c-mint-green);
    position: absolute;
    left: 0;
    bottom: calc(50% - 45px);
    height: calc(50% - 30px);
  }

  .item:after {
    content: " ";
    border-left: 1px solid var(--vt-c-mint-green);
    position: absolute;
    left: 0;
    top: calc(50% + 45px);
    height: calc(50% - 45px);
  }
}
</style>
