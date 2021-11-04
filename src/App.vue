<template>
  <TheHeader />
  <ThePortfolioPage />
  <TheFooter />
</template>

<script>
import TheHeader from "./components/TheHeader"
import TheFooter from "./components/TheFooter"
import ThePortfolioPage from "./pages/PortfolioPage"
export default {
  name: 'App',
  components: {
    TheHeader,
    ThePortfolioPage,
    TheFooter
  }
}
</script>

<style lang="scss">
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  html {
    font-size: 62.5%;
  }
  body {
    background-color: $color-background;
  }
</style>


