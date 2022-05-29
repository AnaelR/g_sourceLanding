<template>
  <div class="dark-bg">
    <div class="first-section">
      <img
          class="logo"
          src="@/assets/images/logo_light.png"
          alt="Logo extension Source"
      />
      <div class="first-section__centered">
        <h1>
          Créez des espaces de discussion pertinants en vérifiant vos sources
        </h1>
        <p>
          Source est une extension web de Twitter qui vous permettra de vérifier
          le contenu d’un tweet à l’aide d’un système de fiabilité de
          l’information qui n’a jamais été aussi objectif.
        </p>
        <ButtonExtension class="cta-button"/>
      </div>
    </div>
    <div class="second-section">
      <h2>Participez à l’élaboration d’un débat plus sain</h2>
      <p>
        Source? s’utilise directement sur l’application web de Twitter et lorem
        ipsum dolore sit amet
      </p>
      <img src="@/assets/images/video.png" alt="Video"/>
    </div>
    <svg
        class="cta-bottom"
        width="39"
        height="23"
        viewBox="0 0 39 23"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
    >
      <path
          d="M36.4457 6.45577L36.4539 6.46331L21.8722 21.05L21.8718 21.0503C21.2765 21.6465 20.425 22 19.5045 22C18.5818 22 17.722 21.645 17.1282 21.0503L17.128 21.0502L2.54591 6.45523L2.55435 6.4475L1.81789 5.70912C1.29827 5.18814 1 4.53295 1 3.82916C1 2.34925 2.33539 1 4.17565 1C5.12527 1 5.95383 1.37545 6.53278 1.95693L7.21001 2.63711L7.2206 2.6274L18.7883 14.1967L19.4955 14.904L20.2026 14.1967L31.7704 2.62733L31.7852 2.64094L32.4623 1.95267C33.028 1.37768 33.8623 1 34.8153 1C36.657 1 38 2.3506 38 3.83751C38 4.54129 37.7017 5.19648 37.1821 5.71746L36.4457 6.45577Z"
          fill="white"
          stroke="black"
          stroke-width="2"
      />
    </svg>
  </div>
</template>

<script>
import ButtonExtension from "./Buttons/ButtonExtension.vue";

export default {
  components: {
    ButtonExtension,
  },
};
</script>

<style lang="scss" scoped>
.dark-bg {
  background-image: url(@/assets/images/header-haut.png),
  url(@/assets/images/header-fond-bas.png);
  background-position: top right, bottom left;
  background-repeat: no-repeat, no-repeat;
  background-size: 60%, 70%;
  overflow-y: hidden;
  min-height: 100vh;
  background-color: $primary-color;

  .cta-bottom {
    position: absolute;
    bottom: 45px;
    right: 0;
    left: 0;
    margin: auto;
  }

  .first-section {
    .logo {
      max-width: 40px;
      margin-top: 45px;
    }

    display: flex;
    flex-direction: column;
    position: relative;
    height: 100vh;
    margin-left: 10%;
    color: $secondary-color;

    &__centered {
      display: flex;
      flex-direction: column;
      margin: auto 0;

      h1 {
        max-width: 550px;
        margin-bottom: 25px;
      }

      p {
        max-width: 550px;
        font-size: $subtitle-size;
        line-height: 1.5;
        margin-bottom: 45px;
      }
    }
  }

  .second-section {
    display: flex;
    text-align: center;
    flex-direction: column;
    color: $secondary-color;
    width: 60%;
    padding: 10% 0;
    margin: auto;

    h2 {
      font-size: $h2-size;
      font-weight: bold;
      margin-bottom: 35px;
    }

    p {
      margin-bottom: 65px;
    }

    img {
      margin: 0 auto;
      max-width: 700px;
    }
  }
}
</style>