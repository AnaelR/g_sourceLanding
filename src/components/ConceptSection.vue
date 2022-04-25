<template>
    <div class="">
        <FirstPart />
        <SecondPart />
        <ThirdPart />
    </div>
</template>
<script>
import FirstPart from './Concept/FirstPart.vue'
import SecondPart from './Concept/SecondPart.vue'
import ThirdPart from './Concept/ThirdPart.vue'
export default {
  components: {
    FirstPart,
    SecondPart,
    ThirdPart,
  }
}
</script>
<style lang="scss" scoped>
    .section {
        padding: $margin-height $margin-width;
    }
</style>