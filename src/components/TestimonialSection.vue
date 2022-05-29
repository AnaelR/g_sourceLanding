<template>
  <div class="testimonial">
    <div class="testimonial__content">
      <h2>Ils y contribuent</h2>
      <p>
        De nombreux utilisateurs utilisent Source? comme outil de vérification
        de l’information sur Twitter et quelle que soit la raison et son
        utilisation, tous y trouvent leur compte et recommendent l’extension
        pour un environnement ,umérique plus sain.
      </p>
      <TestimonialSlider />
    </div>
    <div class="faq">
      <h2>FAQs</h2>
      <p>
        Vous avez une question sur l”utilisation de Source? ou bien sur comment
        est maintenu le plug-in ? N’hésitez pas à consulter les réponses aux
        questions les plus fréquentes ou posez-nous la vôtre directement via
        notre page de contact !
      </p>
      <TestimonialFaq />
    </div>
  </div>
</template>

<script>
import TestimonialFaq from "./Testimonial/TestimonialFaq.vue";
import TestimonialSlider from "./Testimonial/TestimonialSlider.vue";
export default {
  components: {
    TestimonialSlider,
    TestimonialFaq,
  },
};
</script>

<style lang="scss" scoped>
.testimonial {
  background-color: $primary-color;
  padding: 10% 0;
  overflow-x: hidden;
  h2 {
    margin-bottom: 25px;
  }
  p {
    line-height: 1.5;
    font-size: 16px;
    max-width: 800px;
  }
  &__content,
  .faq {
    color: $secondary-color;
    margin-left: 10%;
    width: 80%;
  }
}
</style>