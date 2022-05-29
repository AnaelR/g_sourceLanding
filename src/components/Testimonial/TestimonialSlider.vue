<template>
  <div class="slider">
    <div class="slider__container">
      <div class="tweet">
        <div class="tweet__heading">
          <img src="@/assets/images/pp_hugo.png" alt="pp user"/>
          <h3>Hugo Clément</h3>
        </div>
        <p>
          “Cette député LR dénonce à la télévision une « doxa » sur le
          changement climatique et demande des preuves du phénomène, estimant
          que la science « n’est pas unanime ». Propos irresponsables. La
          science est unanime à ce sujet, et ce depuis de longues années.”
        </p>
      </div>
      <div class="tweet">
        <div class="tweet__heading">
          <img src="@/assets/images/profil_picture.png" alt="pp user"/>
          <h3>PauBrg</h3>
        </div>
        <p>
          “J’ai été très étonnée de voir qu’une source existait pour justifier un tel argument. Pourtant en cherchant de
          mon côté j’ai moi aussi trouvé d’autres sources qui ont la même conclusion. Je peux dire que j’ai appris
          quelque chose aujourd’hui.”
        </p>
      </div>
      <div class="tweet">
        <div class="tweet__heading">
          <img src="@/assets/images/pp_alex.png" alt="pp user"/>
          <h3>AlexPTT</h3>
        </div>
        <p>
          “Je ne pensais pas être exposé à autant de fake. news. Il est important de garder une neutralité avec les
          informations que je peux trouver sur Twitter. J’ai tendance à réagir à chaud. Mais avec les différentes
          sources disponibles je modère mon propos.”
        </p>
      </div>
    </div>
    <ul>
      <li :class="(sliderStep === 1) ? 'active' : ''" @click="previousSlide"></li>
      <li :class="(sliderStep === 0) ? 'active' : ''" @click="nextSlide"></li>
    </ul>
  </div>
</template>

<script>
import gsap from "gsap";

export default {
  data() {
    return {
      sliderStep: 0,
      sliderTimeline: null,
    }
  },
  mounted() {
    this.sliderTimeline = gsap.timeline({paused: true}).to(".slider__container", {
      duration: 0.5,
      x: "-30vw",
    })
  },
  methods: {
    nextSlide() {
      if (this.sliderStep === 1) return
      this.sliderTimeline.play()
      this.sliderStep++
    },
    previousSlide() {
      if (this.sliderStep === 0) return
      this.sliderTimeline.reverse()
      this.sliderStep--
    }
  }
};
</script>

<style lang="scss" scoped>
.slider {
  margin: 50px 0;

  &__container {
    display: flex;
    margin-bottom: 45px;
    width: max-content;
    gap: 40px;

    .tweet {
      padding: 25px;
      border: 2px solid $secondary-color;
      max-width: 32vw;
      border-radius: 15px;

      p {
        font-size: 16px;
        color: #666666;
      }

      &__heading {
        display: flex;
        align-items: center;
        gap: 20px;
        margin-bottom: 25px;

        img {
          max-width: 75px;
        }

        h3 {
          font-size: $h3-size;
          color: $accent-color;
        }
      }
    }
  }

  ul {
    display: flex;
    justify-content: center;
    gap: 25px;

    li {
      text-decoration: none;
      height: 19px;
      width: 19px;
      background-color: $accent-color;
      border-radius: 50%;
    }

    .active {
      cursor: pointer;
      background-color: rgba(214, 26, 136, 0.3);
    }
  }
}
</style>