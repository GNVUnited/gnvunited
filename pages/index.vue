<template>
  <div class="container">
    <article>
      <h1 class="text-4xl">{{ page.title }}</h1>
      <nuxt-content :document="page" class="p-4" />
      <img
        src="~/assets/vigil.png"
        alt="Facbook event screenshot"
        class="max-w-full md:max-w-lg"
      />
    </article>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  async asyncData({ $content }) {
    const page = await $content('home').fetch()

    return {
      page
    }
  }
})
</script>

<style>
.container {
  @apply min-h-screen flex justify-center text-center mx-auto;
}
</style>
