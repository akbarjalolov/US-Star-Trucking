<template>
  <div>
    <main-slider />
    <steps/>
    <us-map/>
    <reviews/>
  </div>
</template>

<script>
import mainSlider from "@/components/main-slider.vue"
import steps from "@/components/steps.vue"
import usMap from "@/components/us-map.vue"
import reviews from "@/components/reviews.vue"
  export default {
    components: {
      mainSlider,
      steps,
      usMap,
      reviews
    },
  }
</script>

<style lang="scss" scoped></style>
