<template>
    <div class="section">
        <img src="@/assets/images/logo-source-black.png" alt="">
        <h3>Prêt à utiliser Source ?</h3>
        <p>Liez votre compte Twitter à Source en quelques clics et découvrez une toute nouvelle expérience du réseau social.</p>
        <ButtonExtension style="margin: auto;" />
    </div>
</template>
<script>
import ButtonExtension from './Buttons/ButtonExtension.vue'
export default {
  components: { ButtonExtension },
    
}
</script>
<style lang="scss" scoped>
    .section {
        padding: $margin-height $margin-width;
        text-align: center;
        width: 50%;
        margin: auto;

        h3 {
            font-size: 36px;
            font-weight: 500;
            margin-top: 27px;
            margin-bottom: 18px;
        }

        p {
            width: 70%;
            margin: auto;
            margin-bottom: 44px;
        }

        img {
            width: 130px;
            height: 126px;
            filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
        }
    }
</style>