<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Blurb from "./components/Blurb.vue";
</script>

<template>
  <div class="container lg:px-80 lg:mx-auto px-2">
    <header>
      <div class="mx-auto pt-10 border-b-2 ">
        <Blurb/>
        <div class="flex gap-10 py-2 justify-evenly">
          <RouterLink class="navLink" to="/">Home</RouterLink>
          <a target="_blank" class="navLink" href="https://app.currentlynotes.com">Currently Notes</a>
        </div>
      </div>
    </header>

    <RouterView />
  </div>
</template>

<style scoped>
.navLink {
  @apply hover:font-semibold hover:scale-110 transition-all text-zinc-800 decoration-8
}
</style>
