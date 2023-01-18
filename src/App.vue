<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Blurb from "./components/Blurb.vue";
</script>

<template>
  <div class="container mx-auto py-5">
    <Blurb/>
    <RouterView />
  </div>
</template>

<style scoped>
.navLink {
  @apply hover:font-semibold hover:scale-110 transition-all text-zinc-800 decoration-8
}
</style>
