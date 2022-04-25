<template>
  <div class="dark-bg">
    <div class="first-section">
      <img src="@/assets/images/logo_light.png" alt="Logo extension Source" />
      <h1>
        Créez des espaces de discussion pertinants en vérifiant vos sources
      </h1>
      <p>
        Source est une extension web de Twitter qui vous permettra de vérifier
        le contenu d’un tweet à l’aide d’un système de fiabilité de
        l’information qui n’a jamais été aussi objectif.
      </p>
      <a href="#" class="cta-extension">Ajouter l'extension à Chrome</a>
      <svg
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
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.dark-bg {
  min-height: 100vh;
  background-color: $primary-color;
  .first-section {
    width: 100vh;
    margin-left: 10%;
    color: $secondary-color;
    h1{
      max-width: 550px;
      margin-bottom: 25px;
    }
    p {
      max-width: 550px;
      font-size: $subtitle-size;
      line-height: 1.5;
    }
  }
}
</style>