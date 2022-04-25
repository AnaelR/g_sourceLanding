<template>
  <a class="cta-extension" href="#">Ajouter à Chrome</a>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.cta-extension {
  padding: 10px 25px;
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
}
</style>