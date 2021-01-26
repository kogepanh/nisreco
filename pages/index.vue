<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">nuxt-templete</h1>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 75vh;
  margin: 0 auto;
  text-align: center;
}

.title {
  display: block;
  font-size: 100px;
  font-weight: 300;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  padding-bottom: 15px;
  font-weight: 300;
  color: #fff;
}

.links {
  padding-top: 15px;
}
</style>
