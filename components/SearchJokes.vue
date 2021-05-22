<template>
  <form @submit.prevent="onSubmit" >
    <input class="bg-gray-700 p-2 rounded" type="text" v-model="text" placeholder="Search Jokes..." />
    <input class="bg-green-900 rounded p-2" type="submit" value="Search Jokes" />
  </form>
</template>

<script>
export default {
  name: "SearchJokes",
  data() {
    return {
      text: "",
    };
  },
  methods: {
    onSubmit() {
      this.$emit("search-text", this.text);
      this.text = "";
    },
  },
};
</script>

<style>
</style>