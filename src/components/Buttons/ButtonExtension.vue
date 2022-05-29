<template>
  <a class="cta-extension" href="">Ajouter à Chrome</a>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.cta-extension {
  display: block;
  padding: 10px 25px;
  transition: background-color 0.2s;
  background-color: $accent-color;
  color: $secondary-color;
  text-decoration: none;
  border-radius: 15px;
  width: fit-content;
  height: 31px;

  &::before {
    content: url("@/assets/icons/chrome.svg");
    display: inline-flex;
    vertical-align: middle;
    margin-right: 20px;
    scale: 0.8;
    margin-top: -2px;
  }

  &:hover {
    transition: background-color 0.5s;
    background-color: #961963;

    &::before {
      transition: transform 0.5s ease-in-out;
      transform: rotate(360deg);
    }
  }
}
</style>