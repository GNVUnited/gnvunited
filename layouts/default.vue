<template>
  <div>
    <Nav />
    <nuxt />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Nav from '~/components/Nav.vue'

export default Vue.extend({
  components: {
    Nav
  }
})
</script>

<style>
body {
  @apply bg-white;
}
</style>
