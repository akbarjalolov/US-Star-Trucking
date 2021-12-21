<template>
  <div>
    <main-slider />
    <steps/>
    <us-map/>
  </div>
</template>

<script>
import mainSlider from "@/components/main-slider.vue"
import steps from "@/components/steps.vue"
import usMap from "@/components/us-map.vue"
  export default {
    components: {
      mainSlider,
      steps,
      usMap
    },
  }
</script>

<style lang="scss" scoped></style>
