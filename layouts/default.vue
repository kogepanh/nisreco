<template>
  <div class="layout">
    <Header class="layout__header" />
    <Nuxt class="layout__main" />
    <Footer class="layout__footer" />
  </div>
</template>

<style>
.layout__header {
  min-height: 20vh;
  font-size: 0.5rem;
}

.layout__main {
  width: 100%;
}

.layout__footer {
  min-height: 5vh;
}
</style>
