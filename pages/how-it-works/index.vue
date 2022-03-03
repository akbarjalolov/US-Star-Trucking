<template>
<div>
  <div class="how-it-works common pt-54 pb-54">
    <div class="container mt-100">
      <div class="row"
      data-aos="fade-right"
          data-aos-once="true"
          data-aos-anchor-placement="center-bottom"
          data-aos-duration="600"
      >
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
            Book your vehicle transportation online or by phone.
          </h5>
          <p>
           It's simple to send a car using US Star Trucking! 
<br><br>

Using our online car shipping quotation tool, you just submit some necessary details of your shipment such as pickup and destination zip codes, trailer type, vehicle details and  shipping dates.
<br><br>

Then one of our available agents will manually calculate the best competitive quotes and get back to you shortly via email and  phone call.  Then you can go ahead and compare our prices and services (we know you want to!) — we’re sure you’ll find our prices very competitive.
          </p>
        </div>
      </div>
      <div class="row flex-column-reverse flex-lg-row mb-79"
      data-aos="fade-left"
          data-aos-once="true"
          data-aos-anchor-placement="center-bottom"
          data-aos-duration="600"
      >
         <div class="col-12 col-lg-9">
          <h5 class="mb-8">
            We pick up your vehicle
          </h5>
          <p>
           US Star Trucking experts will work with you to set up a pick-up time and date that works best for you. As a direct customer of our company, we do our best to work around your schedule and assign only trusted truckers for your shipment.
<br><br>

When your trucker arrives, both of you will inspect your car together and sign a Bill of Lading. Then  the assigned trucker will take care of the rest.  
<br><br>
While your car is enjoying its journey, you can check in with your trucker directly  as often as  you wish to get updates.
          </p>
        </div>
         <div class="col-12 col-lg-3">
          <div class="text-center text-lg-left">
            <img class="img-fluid" src="/images/second-step.png" alt="">
          </div>
        </div>
        
      </div>
      <div class="row" data-aos="fade-right"
          data-aos-once="true"
          data-aos-anchor-placement="center-bottom"
          data-aos-duration="600">
         <div class="col-12 col-lg-3">
          <div class="text-center text-lg-left">
            <img class="img-fluid" src="/images/third-step.png" alt="">
          </div>
        </div>
        <div class="col-12 col-lg-9 mb-79">
          <h5 class="mb-8">
            Receive your vehicle 
          </h5>
          <p>
            You will receive a short update from the driver some time before the drop off which should leave you with enough preparation time.  Then your assigned trucker will deliver your vehicle to your doorsteps (as we offer door-to-door service) or any other drop off location of your convenience. <br><br> After a careful inspection to make sure everything looks good, you’ll simply sign the  Bill of landing
to accept your delivery. That’s it!
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