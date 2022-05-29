<template>
  <HeadingSection />
  <ConceptSection />
  <TestimonialSection />
  <CallToActionSection />
  <FooterSection />
</template>

<script>
import TestimonialSection from "./components/TestimonialSection.vue";
import CallToActionSection from "./components/CallToActionSection.vue";
import ConceptSection from "./components/ConceptSection.vue";
import HeadingSection from "./components/HeadingSection.vue";
import FooterSection from "./components/FooterSection.vue";

export default {
  name: "App",
  components: {
    HeadingSection,
    ConceptSection,
    CallToActionSection,
    FooterSection,
    TestimonialSection,
  },
};
</script>

<style lang="scss">
#app {
  margin-top: 10px;
}
</style>
