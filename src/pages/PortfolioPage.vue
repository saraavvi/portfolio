<template>
  <div class="container">
    <LandingSection class="section" />
    <AboutSection class="section" />
    <PortfolioSection class="section" />
    <ContactSection class="section" />
  </div>
</template>

<script>
import LandingSection from "../components/LandingSection";
import AboutSection from "../components/AboutSection";
import PortfolioSection from "../components/PortfolioSection";
import ContactSection from "../components/ContactSection";
export default {
  components: {
    LandingSection,
    AboutSection,
    PortfolioSection,
    ContactSection,
  },
};
</script>

<style scoped lang="scss">
.container {
  display: flex;
  flex-direction: column;
  margin: 0 16rem 0 16rem;

  .section {
    margin-bottom: 10rem;
  }
}
</style>
