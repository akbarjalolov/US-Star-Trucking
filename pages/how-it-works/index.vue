<template>
<div>
  <div class="how-it-works common pt-54 pb-54">
    <div class="container mt-100">
      <div class="row">
        <div class="col-12 mb-48">
          <div class="d-flex align-items-center">
            <svg
              width="40"
              height="40"
              viewBox="0 0 40 40"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M20 35.6C28.6156 35.6 35.6 28.6156 35.6 20C35.6 11.3844 28.6156 4.4 20 4.4C11.3844 4.4 4.4 11.3844 4.4 20C4.4 28.6156 11.3844 35.6 20 35.6ZM20 39.5C30.7696 39.5 39.5 30.7696 39.5 20C39.5 9.23045 30.7696 0.5 20 0.5C9.23045 0.5 0.5 9.23045 0.5 20C0.5 30.7696 9.23045 39.5 20 39.5Z"
                fill="white"
              />
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M20 10.25C18.9231 10.25 18.05 11.1231 18.05 12.2C18.05 13.277 18.9231 14.15 20 14.15C21.077 14.15 21.95 13.277 21.95 12.2C21.95 11.1231 21.077 10.25 20 10.25ZM20 18.05C18.9231 18.05 18.05 18.9231 18.05 20V27.8C18.05 28.877 18.9231 29.75 20 29.75C21.077 29.75 21.95 28.877 21.95 27.8V20C21.95 18.9231 21.077 18.05 20 18.05Z"
                fill="white"
              />
            </svg>
            <h2 class="ml-18">How it works ?</h2>
          </div>
        </div>
        <div class="col-12 col-lg-3">
          <div class="text-center text-lg-left">
            <img class="img-fluid" src="/images/first-step.png" alt="">
          </div>
        </div>
        <div class="col-12 col-lg-9 mb-79">
          <h5 class="mb-8">
            Schedule a car shipment online or over the phone.
          </h5>
          <p>
            Schedule a vehicle shipment with Nexus and you'll be surprised at how easy it is! All you have to do is enter your car pickup and car delivery zip codes in our online car shipping quote tool (or give that information to one of our dedicated vehicle transport agents), select your vehicle type and size, choose between open or enclosed auto transport, and pick from a variety of different car shipment scheduling dates.

            You're bound to find a fair shipping rate that works for you, or you can pay a bit more for expedited enclosed vehicle transport. It all depends on your needs and the driver availability of our network of car haulers. Reserve your car shipment with a refundable $0 reservation fee. Our low-risk car delivery service is suitable for any budget.
          </p>
        </div>
      </div>
      <div class="row flex-column-reverse flex-lg-row mb-79">
         <div class="col-12 col-lg-9">
          <h5 class="mb-8">
            We pick up your car and the vehicle transport journey begins
          </h5>
          <p>
            One of our expert Nexus auto transport coordinators will work with you to arrange a vehicle pickup date and time which works best for you. When you ship a car direct with Nexus, we do our very best to work around your schedule!

Just prep your vehicle for car hauling by cleaning it inside and out, removing valuable personal items, and making sure there's at least a quarter tank of gas for loading and unloading it off of the car hauler. On car pickup day, you or someone you authorize through Nexus will inspect your vehicle with your driver to notate preexisting damages and other concerns. Once the Bill of Lading and the inspection report are signed, your car will be on its way!
          </p>
        </div>
         <div class="col-12 col-lg-3">
          <div class="text-center text-lg-left">
            <img class="img-fluid" src="/images/second-step.png" alt="">
          </div>
        </div>
        
      </div>
      <div class="row">
         <div class="col-12 col-lg-3">
          <div class="text-center text-lg-left">
            <img class="img-fluid" src="/images/third-step.png" alt="">
          </div>
        </div>
        <div class="col-12 col-lg-9 mb-79">
          <h5 class="mb-8">
            Our car hauling service delivers your vehicle to its destination.
          </h5>
          <p>
            You can contact your car transporter at any time during your vehicle shipment to ask questions about arrival times and anything else that may be on your mind. Our vehicle transport truckers go through rigorous safety and procedural training to ensure that your car is safe every step of the way!

The vehicle transport hauler will come as close to your address as safely and legally possible. Any balance due on your vehicle shipment can be paid to your trucker upon arrival. You or someone you appoint will conduct a final vehicle inspection, sign off on a Bill of Lading, and you're done! Shipping is complex with other car moving companies. But, it’s as simple as 1, 2, 3 with Nexus.
          </p>
        </div>
      </div>
    </div>
  </div>
    <usMap/>

  </div>
</template>

<script>
import usMap from "@/components/us-map.vue"
import AOS from "aos";
import "aos/dist/aos.css";
export default {
  layout: "pages",

  components: {
    usMap
  },

  mounted(){
    
    AOS.init();

  },
};
</script>