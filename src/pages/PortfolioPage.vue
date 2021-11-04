<template>
    <h2> portfolio page </h2>
    <LandingSection />
    <AboutSection />
    <PortfolioSection />
    <ContactSection />
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