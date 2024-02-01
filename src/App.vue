<script>
import AppHeader from "./components/AppHeader.vue"
import AppMainContent from "./components/AppMainContent.vue"
import AppSpam from "./components/AppSpam.vue"
import AppFooterTop from "./components/Footer/AppFooterTop.vue"
import AppFooterBottom from "./components/Footer/AppFooterBottom.vue"

export default {

  name: "Vite-Comics",
  components: {
    AppHeader,
    AppMainContent,
    AppSpam,
    AppFooterTop,
    AppFooterBottom,
  },
};
</script>

<template>
  <AppHeader />
  <AppMainContent />
  <AppSpam />
  <footer>
    <AppFooterTop />
    <AppFooterBottom />
  </footer>
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