<template>
  <HeadingSection />
  <ConceptSection />
  <CallToActionSection />
  <FooterSection />
</template>

<script>
import CallToActionSection from './components/CallToActionSection.vue'
import ConceptSection from './components/ConceptSection.vue'
import HeadingSection from './components/HeadingSection.vue'
import FooterSection from './components/FooterSection.vue'

export default {
  name: "App",
  components: {
    HeadingSection,
    ConceptSection,
    CallToActionSection,
    FooterSection
  }
}
</script>

<style lang="scss">
#app {
  margin-top: 10px;
}
</style>
