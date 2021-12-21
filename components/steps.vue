<template>
  <div class="steps pt-54 pb-54">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h1 class="section-titles">
            <svg
              width="48"
              height="48"
              viewBox="0 0 48 48"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M36.5061 4.95605C40.6273 3.23889 44.7617 7.37333 43.0446 11.4945L31.1975 39.9274C28.8806 45.488 20.731 44.5481 19.7407 38.6061L18.2627 29.7379L9.3945 28.2599C3.45252 27.2696 2.51265 19.12 8.0732 16.8031L36.5061 4.95605ZM39.3522 9.95605C39.6957 9.13181 38.8688 8.30493 38.0446 8.64836L9.61166 20.4954C7.75814 21.2677 8.07144 23.9842 10.0521 24.3143L18.9203 25.7924C20.6062 26.0733 21.9273 27.3945 22.2082 29.0803L23.6863 37.9485C24.0164 39.9292 26.7329 40.2425 27.5052 38.3889L39.3522 9.95605Z"
                fill="white"
              />
            </svg>
            Easy steps
          </h1>
        </div>
        <div class="col-12 mt-69" v-for="(item, index) in steps" :key="index">
          <div class="d-flex align-items-center">
            <div>
              <h2 class="mr-16">{{ index + 1 }}</h2>
            </div>
            <div>
              <h3 class="mb-12">
                {{ item.title }}
              </h3>
              <p>
                {{ item.description }}
              </p>
            </div>
          </div>
        </div>
        <div class="col-12 text-right mt-24">
            <div class="d-flex justify-content-end">
 <button class="white-btn d-flex align-item-center justify-content-right">LEARN MORE
                 <lottie-player
                 class="ml-4"
  autoplay
  loop
  style="width:30px"
  src="https://assets2.lottiefiles.com/packages/lf20_9kxnutyd.json"
  speed="1"
  debug
></lottie-player>
            </button>
            </div>
           
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      steps: [
        {
          title: "How trucking works?",
          description:
            "Trucking is a cash flow-intensive business. You are always buying fuel, making insurance payments, making truck payments, and so on. Unless you get quick-pays, shippers and brokers can pay invoices in 15 to 30 days. ... Many factoring companies provide fuel advances, cards, and other services as well.",
        },
         {
          title: "How trucking works?",
          description:
            "Trucking is a cash flow-intensive business. You are always buying fuel, making insurance payments, making truck payments, and so on. Unless you get quick-pays, shippers and brokers can pay invoices in 15 to 30 days. ... Many factoring companies provide fuel advances, cards, and other services as well.",
        },
         {
          title: "How trucking works?",
          description:
            "Trucking is a cash flow-intensive business. You are always buying fuel, making insurance payments, making truck payments, and so on. Unless you get quick-pays, shippers and brokers can pay invoices in 15 to 30 days. ... Many factoring companies provide fuel advances, cards, and other services as well.",
        },
      ],
    };
  },
};
</script>