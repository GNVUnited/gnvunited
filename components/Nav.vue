<template>
  <nav class="flex items-center justify-center flex-wrap p-6">
    <div class="flex items-center">
      <h1 class="title md:text-6xl text-4xl">GNV United</h1>
      <logo />
    </div>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'
import Logo from '~/components/Logo.vue'

export default Vue.extend({
  components: {
    Logo
  }
})
</script>
