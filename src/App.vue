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


