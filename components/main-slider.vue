<template>
  <div class="main-slider">
    <div class="gradient d-flex align-items-center">
      <div class="buttons">
        <svg
          @click="prev"
          class="prev"
          width="62"
          height="124"
          viewBox="0 0 62 124"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle cy="62" r="61.5" stroke="white" stroke-opacity="0.5" />
          <path
            d="M40 62.5C40.2761 62.5 40.5 62.2761 40.5 62C40.5 61.7239 40.2761 61.5 40 61.5L40 62.5ZM19.6464 61.6464C19.4512 61.8417 19.4512 62.1583 19.6464 62.3536L22.8284 65.5355C23.0237 65.7308 23.3403 65.7308 23.5355 65.5355C23.7308 65.3403 23.7308 65.0237 23.5355 64.8284L20.7071 62L23.5355 59.1716C23.7308 58.9763 23.7308 58.6597 23.5355 58.4645C23.3403 58.2692 23.0237 58.2692 22.8284 58.4645L19.6464 61.6464ZM40 61.5L20 61.5L20 62.5L40 62.5L40 61.5Z"
            fill="white"
            fill-opacity="0.5"
          />
        </svg>
        <svg
          @click="next"
          class="next"
          width="62"
          height="124"
          viewBox="0 0 62 124"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle cy="62" r="61.5" stroke="white" stroke-opacity="0.5" />
          <path
            d="M40 62.5C40.2761 62.5 40.5 62.2761 40.5 62C40.5 61.7239 40.2761 61.5 40 61.5L40 62.5ZM19.6464 61.6464C19.4512 61.8417 19.4512 62.1583 19.6464 62.3536L22.8284 65.5355C23.0237 65.7308 23.3403 65.7308 23.5355 65.5355C23.7308 65.3403 23.7308 65.0237 23.5355 64.8284L20.7071 62L23.5355 59.1716C23.7308 58.9763 23.7308 58.6597 23.5355 58.4645C23.3403 58.2692 23.0237 58.2692 22.8284 58.4645L19.6464 61.6464ZM40 61.5L20 61.5L20 62.5L40 62.5L40 61.5Z"
            fill="white"
            fill-opacity="0.5"
          />
        </svg>
      </div>
      <div class="container">
        <div class="row">
          <div class="col-12 relative text-center text-lg-left">
            <!-- <h1 class="mb-8">Competitive rates, safety, and reliable on-time</h1> -->
            <div class="content4">
              <div class="content4__container d-flex justify-content-lg-start justify-content-center">
                <p class="content4__container__text">WE SHIP </p>
                <ul class="content4__container__list">
                  <li class="content4__container__list__item pl-18">CARS </li>
                  <li class="content4__container__list__item pl-18">SUVS </li>
                  <li class="content4__container__list__item pl-18">TRUCKS </li>
                  <li class="content4__container__list__item pl-18">MOTORCYCLES </li>
                </ul>
               
              </div>
            </div>
        
              <h6 class="mb-16">
                Deliver your vehicles nationally on time with no hassle!</h6>
       
            <div
              data-aos="fade-left"
              data-aos-delay="3000"
              data-aos-once="true"
            >
              <a
                target="_blank"
                href="https://apps.msgplane.com/quote/usst?id=24bc1d17-a5e2-45a0-8d54-a87a9f532e88"
              >
                <button class="white-btn">GET A QUOTE</button>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>

    <VueSlickCarousel v-bind="settings" ref="mainSlider" class="main-slider">
      <div v-for="(item, index) in mainPics" :key="index">
        <video autoplay muted loop v-if="item.type === 'video'">
          <source :src="item.src" type="video/mp4" />
          {{ item.alt }}1
        </video>
        <img
          :src="item.src"
          v-if="item.type === 'picture'"
          draggable="false"
          :alt="item.alt"
        />
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";
import Typewriter from "typewriter-vue";
export default {
  components: {
    Typewriter,
  },

  data() {
    return {
      video: "static/images/video.mp4",
      settings: {
        dots: true,
        dotsClass: "slick-dots custom-dot-class",
        infinite: true,
        autoplay: true,
        autoplaySpeed: 14000,
        speed: 1000,
        slidesToShow: 1,
        slidesToScroll: 1,
        arrows: false,
      },

      mainPics: [
        {
          src: "/images/video2.mp4",
          alt: "Transportation pics",
          type: "video",
        },
        {
          src: "/images/main2.jpg",
          alt: "Transportation pics",
          type: "picture",
        },
        {
          src: "/images/video4.mp4",
          alt: "Transportation pics",
          type: "video",
        },
        {
          src: "/images/main.png",
          alt: "Transportation pics",
          type: "picture",
        },
        {
          src: "/images/main3.jpg",
          alt: "Transportation pics",
          type: "picture",
        },
      ],
    };
  },

  methods: {
    prev() {
      this.$refs.mainSlider.prev();
    },

    next() {
      this.$refs.mainSlider.next();
    },
  },
  mounted() {
    AOS.init();
  },
};
</script>