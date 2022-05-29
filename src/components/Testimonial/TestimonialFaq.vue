<template>
  <div class="faq-component">
    <div @click="toggleAnswer(0)" class="faq-component__element">
      <div class="faq-component__element__heading">
        <h4>Qu'est-ce qu'une source d’information ?</h4>
        <svg
            width="19"
            height="19"
            viewBox="0 0 19 19"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
        >
          <path d="M9.5 0L9.5 19M0 9.5H19" stroke="white" stroke-width="3"/>
        </svg>
      </div>
      <div class="faq-component__element__content">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique est
          ducimus numquam voluptate, sed nostrum quas recusandae, saepe sit
          consectetur voluptatibus, ut repellat iure tenetur iste quaerat maxime
          exercitationem magnam?
        </p>
      </div>
    </div>
    <div @click="toggleAnswer(1)" class="faq-component__element">
      <div class="faq-component__element__heading">
        <h4>Comment est vérifiée la fiabilité des sources ?</h4>
        <svg
            width="19"
            height="19"
            viewBox="0 0 19 19"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
        >
          <path d="M9.5 0L9.5 19M0 9.5H19" stroke="white" stroke-width="3"/>
        </svg>
      </div>
      <div class="faq-component__element__content">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique est
          ducimus numquam voluptate, sed nostrum quas recusandae, saepe sit
          consectetur voluptatibus, ut repellat iure tenetur iste quaerat maxime
          exercitationem magnam?
        </p>
      </div>
    </div>
    <div @click="toggleAnswer(2)" class="faq-component__element">
      <div class="faq-component__element__heading">
        <h4>Comment sont comptabilisés les votes sur la barre de véracité ?</h4>
        <svg
            width="19"
            height="19"
            viewBox="0 0 19 19"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
        >
          <path d="M9.5 0L9.5 19M0 9.5H19" stroke="white" stroke-width="3"/>
        </svg>
      </div>
      <div class="faq-component__element__content">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique est
          ducimus numquam voluptate, sed nostrum quas recusandae, saepe sit
          consectetur voluptatibus, ut repellat iure tenetur iste quaerat maxime
          exercitationem magnam?
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: null,
    }
  },
  mounted() {
    this.items = document.querySelectorAll(".faq-component__element");
  },
  methods: {
    toggleAnswer(index) {
      this.items[index].classList.toggle("active");
    }
  }
};
</script>

<style lang="scss" scoped>
.faq-component {
  margin-top: 32px;

  &__element {
    border-top: 2px solid $secondary-color;
    padding: 25px 0;

    &:nth-last-child(1) {
      border-bottom: 2px solid $secondary-color;
    }

    &__heading {
      display: flex;
      justify-content: space-between;

      svg {
        transition: transform 0.5s;
        transform: rotate(0);
      }
    }

    &__content {
      overflow: hidden;
      max-height: 0;
      transition: max-height 0.6s;

      p {
        margin-top: 24px;
      }
    }
  }

  .active {
    .faq-component__element__content {
      max-height: 100px;
      transition: max-height 0.6s;
    }

    .faq-component__element__heading {
      svg {
        transition: transform 0.6s;
        transform: rotate(135deg);
      }
    }
  }
}
</style>