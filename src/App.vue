<script>
import AppHeader from "./components/AppHeader.vue"
import AppMainContent from "./components/AppMainContent.vue"
import AppFooterTop from "./components/Footer/AppFooterTop.vue"

export default {

  name: "Vite-Comics",
  components: {
    AppHeader,
    AppMainContent,
    AppFooterTop,
  },
};
</script>

<template>
  <AppHeader />
  <AppMainContent />
  <AppFooterTop />
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Open Sans', Open Sans Condensed;
}
</style>