<template>
  <nuxt-link :to="'jokes/' + id">
    <div class="joke border border-dotted p-2 mt-2">
      <p>{{ joke }}</p>
    </div>
  </nuxt-link>
</template>

<script>
export default {
  name: "Joke",
  props: ["joke", "id"],
};
</script>

<style>
</style>