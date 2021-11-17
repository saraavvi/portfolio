<template>
  <TheHeader />
  <ThePortfolioPage />
</template>

<script>
import TheHeader from "./components/TheHeader";
import ThePortfolioPage from "./pages/PortfolioPage";
export default {
  name: "App",
  components: {
    TheHeader,
    ThePortfolioPage,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

html {
  font-size: 62.5%;
  box-sizing: border-box;
}

body {
  background-color: $color-background;
  font-family: $font-primary;

  a {
    outline: none;
    text-decoration: none;
    color: inherit;
  }
}
</style>
