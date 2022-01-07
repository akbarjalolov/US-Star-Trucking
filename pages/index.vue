<template>
  <div>
    <div>
      <main-slider />
    </div>
 <div>
    <steps />
 </div>
    <us-map />
    <reviews />
  </div>
</template>

<script>  
import AOS from "aos";
import "aos/dist/aos.css";

import mainSlider from "@/components/main-slider.vue";
import steps from "@/components/steps.vue";
import usMap from "@/components/us-map.vue";
import reviews from "@/components/reviews.vue";
import partners from "@/components/partners.vue";
export default {
  components: {
    mainSlider,
    steps,
    usMap,
    reviews,
    partners,
  },
   mounted() {
    AOS.init();
  },

};
</script>

<style lang="scss" scoped></style>
