<script>
import AppHeader from "./components/AppHeader.vue"
import AppMainContent from "./components/AppMainContent.vue"
export default {

  name: "Vite-Comics",
  components: {
    AppHeader,
    AppMainContent,
  },
};
</script>

<template>
  <AppHeader />
  <AppMainContent />
</template>

<style>
body {
  font-family: 'Open Sans', Open Sans Condensed;
}
</style>