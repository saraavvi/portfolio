<template>
    <div class="container">
    <LandingSection />
    <AboutSection />
    <PortfolioSection />
    <ContactSection />
    </div>
</template>

<script>
import LandingSection from "../components/LandingSection"
import AboutSection from "../components/AboutSection"
import PortfolioSection from "../components/PortfolioSection"
import ContactSection from "../components/ContactSection"
export default {
    components: {
        LandingSection,
        AboutSection,
        PortfolioSection,
        ContactSection
    }
}
</script>

<style scoped lang="scss">
    .container {
        display: flex;
        flex-direction: column;
        margin: 0 12rem 0 12rem;
    }
</style>