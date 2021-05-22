<template>
  <header class="flex items-center justify-between p-4 bg-gray-700">
    <div>
      <h1 class="text-2xl">Dad Jokes</h1>
    </div>
    <div class="flex space-x-4">
      <nuxt-link class="navbutton" to="/">Home</nuxt-link>
      <nuxt-link class="navbutton" to="/jokes">Jokes</nuxt-link>
      <nuxt-link class="navbutton" to="/about">About</nuxt-link>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style>
@layer base {
  .navbutton {
    @apply py-1 px-3 bg-red-900 rounded;
  }
}
</style>