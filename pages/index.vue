<template>
  <div>
    <main-slider />
    <steps />
    <us-map />
    <reviews />
    <partners/>
    <blog-slider />
    <b-modal id="modal-lg" v-model="discount" size="lg">
    <div class="card pt-76 pb-24 pr-100 pl-100">
      <svg class="logo-rounded" width="120" height="120" viewBox="0 0 120 120" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect x="0.5" y="0.5" width="119" height="119" rx="59.5" fill="#28293A"/>
<path d="M59.5277 57.7455C61.2366 59.0211 38.442 96.681 40.9039 94.9416L59.5277 81.5185L78.1225 94.9416C80.5555 96.681 57.7899 59.0211 59.5277 57.7455C61.2076 56.4699 86.4351 92.4773 85.4793 89.7231L78.1225 68.2694L96.8911 55.0493C99.3241 53.3678 60.1939 59.7169 59.5277 57.7455C58.8615 55.7741 97.0938 46.5548 94.0816 46.5838L71.0553 46.7577L64.0171 25.1591C63.0903 22.3469 61.6421 57.7455 59.5277 57.7455C57.3844 57.7455 55.9072 22.3469 54.9804 25.1591L47.9711 46.7577L24.9159 46.5838C21.9036 46.5548 60.1939 55.8031 59.5277 57.7455C58.8326 59.7459 19.7024 53.3678 22.1064 55.0493L40.875 68.2694L33.5181 89.7231C32.5623 92.4773 57.8188 56.4699 59.5277 57.7455Z" fill="white"/>
<rect x="0.5" y="0.5" width="119" height="119" rx="59.5" stroke="#28293A"/>
</svg>
      <h5 class="mb-8">SAVE UP TO 5% ON YOUR QUOTE?</h5>
      <h6 class="mb-31">
        Enter your email to find out
      </h6>
      <div class="email">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M4.8 12C4.8 8.02355 8.02355 4.8 12 4.8C15.9765 4.8 19.2 8.02355 19.2 12C19.2 12.2199 19.1961 12.9908 18.9649 13.6841C18.8509 14.0262 18.7019 14.2849 18.529 14.4501C18.3775 14.5948 18.1774 14.7 17.85 14.7C17.4866 14.7 17.3118 14.6003 17.1926 14.4784C17.0428 14.3254 16.8828 14.0332 16.7589 13.488C16.5056 12.3735 16.5 10.6978 16.5 8.4C16.5 7.90294 16.0971 7.5 15.6 7.5C15.1031 7.5 14.7002 7.90277 14.7 8.39968C13.9479 7.83475 13.013 7.5 12 7.5C9.51472 7.5 7.5 9.51472 7.5 12C7.5 14.4853 9.51472 16.5 12 16.5C13.3443 16.5 14.5509 15.9105 15.3755 14.976C15.5142 15.2558 15.6874 15.5139 15.9059 15.7372C16.4195 16.2622 17.0884 16.5 17.85 16.5C18.6476 16.5 19.2912 16.2114 19.7726 15.7515C20.2325 15.312 20.5053 14.755 20.6726 14.2534C21.0002 13.2703 21 12.2531 21 12.008V12C21 7.02944 16.9706 3 12 3C7.02944 3 3 7.02944 3 12C3 16.9706 7.02944 21 12 21C13.4352 21 14.7944 20.6634 16.0005 20.064C16.4457 19.8428 16.6272 19.3026 16.406 18.8575C16.1848 18.4124 15.6446 18.2309 15.1995 18.4521C14.2367 18.9305 13.1511 19.2 12 19.2C8.02355 19.2 4.8 15.9764 4.8 12ZM14.7 12C14.7 13.4912 13.4912 14.7 12 14.7C10.5088 14.7 9.3 13.4912 9.3 12C9.3 10.5088 10.5088 9.3 12 9.3C13.4912 9.3 14.7 10.5088 14.7 12Z" fill="#28293A"/>
</svg>

      <el-input class="mb-16" placeholder="Email address" v-model="email"></el-input>
      </div>

      <button class="mb-12 dark-btn">UNLOCK SAVINGS</button>
      <p>
        By providing your information, you agree to our <a href="privacy-policy">privacy policy.</a>
      </p>
    </div>
  </b-modal>
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
import BlogSlider from '../components/blog-slider.vue';
import Partners from '../components/partners.vue';
export default {
  components: {
    mainSlider,
    steps,
    usMap,
    reviews,
    Partners,
    BlogSlider,
  },

  data() {
    return {
      discount: false,
      email: ''
    }
  },

   mounted(){
    
    AOS.init();

    setTimeout(() => {this.discount = true}, 1000)
  },

};
</script>

<style lang="scss" scoped></style>
