<template>
  <section class="container">
    <div>
      <logo/>
      <h1 class="title">
        rescopl
      </h1>
      <h2 class="subtitle">
        a research coordination platform
      </h2>
      <div class="links">
        <a href="https://github.com/Vandivier/rescopl" target="_blank" class="button--grey">GitHub</a>
        <a href="https://nuxtjs.org/" target="_blank" class="button--grey">Nuxt Documentation</a>
        <a href="/bookmarks" class="button--grey">John's Bookmarks</a>
      </div>
      <div class="links">
        <nuxt-link to="/create-idea" class="button--green">Create Idea</nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
    components: {
        Logo
    }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
