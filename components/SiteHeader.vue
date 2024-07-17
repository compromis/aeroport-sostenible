<template>
  <header v-motion-slide-visible-bottom class="header">
    <SiteTitle />
  </header>
</template>

<style lang="scss" scoped>
  svg {
    width: 100%;
    max-width: 650px;
  }

  .header {
    display: flex;
    justify-content: center;
    margin: 7rem 0 2rem;
  }
</style>