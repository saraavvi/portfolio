<template>
  <TheHeader />
  <TheSidebar />
  <ThePortfolioPage />
</template>

<script>
import TheHeader from "./components/TheHeader";
import TheSidebar from "./components/TheSidebar";
import ThePortfolioPage from "./pages/PortfolioPage";
export default {
  name: "App",
  components: {
    TheHeader,
    TheSidebar,
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
  scroll-behavior: smooth;
  scroll-padding-top: 10rem;

  @include respond(tab-land) {
    font-size: 56.29%;
  }
  @include respond(tab-port) {
    font-size: 50%;
  }
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
