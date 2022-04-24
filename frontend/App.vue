<template>
  <div class="App">
    <Auth />
    <Main />
  </div>
</template>

<script lang="ts">
import Main from "./Main.vue"
import Auth from "./Auth.vue"

export default {
  name: "App",
  components: {
    Main,
    Auth,
  },
}
</script>

<style>
html {
  background-color: #303030;
}
</style>
