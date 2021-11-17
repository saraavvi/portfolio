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
  font-size: 1.7rem;
  line-height: 1.8;
  color: $color-font-black;
  width: 80%;
  margin: 0 auto;
  max-width: 180rem;

  .section {
    margin-bottom: 20rem;
  }
}
</style>
