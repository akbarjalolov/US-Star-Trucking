<template>
  <div class="steps pt-54 pb-54">
    <div class="container">
      <div class="row">
        <div
          class="col-12"
          data-aos="fade-up"
          data-aos-once="true"
          data-aos-anchor-placement="center-bottom"
          data-aos-duration="600"
        >
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
            Ship your vehicle in 3 easy steps
          </h1>
        </div>
        <div class="col-12 mt-69" v-for="(item, index) in steps" :key="index">
          <div
            class="d-flex align-items-center"
            data-aos="fade-up"
            data-aos-once="true"
            data-aos-anchor-placement="center-bottom"
            data-aos-duration="600"
          >
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
          <div class="hover-btn d-flex align-item-center justify-content-end">
            <div class="wrapper2">
              <nuxt-link to="/how-it-works" class="cta" href="#">
                <span>LEARN MORE</span>
                <span>
                  <svg
                    width="31px"
                    height="20px"
                    viewBox="0 0 66 43"
                    version="1.1"
                    xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink"
                  >
                    <g
                      id="arrow"
                      stroke="none"
                      stroke-width="1"
                      fill="none"
                      fill-rule="evenodd"
                    >
                      <path
                        class="one"
                        d="M40.1543933,3.89485454 L43.9763149,0.139296592 C44.1708311,-0.0518420739 44.4826329,-0.0518571125 44.6771675,0.139262789 L65.6916134,20.7848311 C66.0855801,21.1718824 66.0911863,21.8050225 65.704135,22.1989893 C65.7000188,22.2031791 65.6958657,22.2073326 65.6916762,22.2114492 L44.677098,42.8607841 C44.4825957,43.0519059 44.1708242,43.0519358 43.9762853,42.8608513 L40.1545186,39.1069479 C39.9575152,38.9134427 39.9546793,38.5968729 40.1481845,38.3998695 C40.1502893,38.3977268 40.1524132,38.395603 40.1545562,38.3934985 L56.9937789,21.8567812 C57.1908028,21.6632968 57.193672,21.3467273 57.0001876,21.1497035 C56.9980647,21.1475418 56.9959223,21.1453995 56.9937605,21.1432767 L40.1545208,4.60825197 C39.9574869,4.41477773 39.9546013,4.09820839 40.1480756,3.90117456 C40.1501626,3.89904911 40.1522686,3.89694235 40.1543933,3.89485454 Z"
                        fill="#FFFFFF"
                      ></path>
                      <path
                        class="two"
                        d="M20.1543933,3.89485454 L23.9763149,0.139296592 C24.1708311,-0.0518420739 24.4826329,-0.0518571125 24.6771675,0.139262789 L45.6916134,20.7848311 C46.0855801,21.1718824 46.0911863,21.8050225 45.704135,22.1989893 C45.7000188,22.2031791 45.6958657,22.2073326 45.6916762,22.2114492 L24.677098,42.8607841 C24.4825957,43.0519059 24.1708242,43.0519358 23.9762853,42.8608513 L20.1545186,39.1069479 C19.9575152,38.9134427 19.9546793,38.5968729 20.1481845,38.3998695 C20.1502893,38.3977268 20.1524132,38.395603 20.1545562,38.3934985 L36.9937789,21.8567812 C37.1908028,21.6632968 37.193672,21.3467273 37.0001876,21.1497035 C36.9980647,21.1475418 36.9959223,21.1453995 36.9937605,21.1432767 L20.1545208,4.60825197 C19.9574869,4.41477773 19.9546013,4.09820839 20.1480756,3.90117456 C20.1501626,3.89904911 20.1522686,3.89694235 20.1543933,3.89485454 Z"
                        fill="#FFFFFF"
                      ></path>
                      <path
                        class="three"
                        d="M0.154393339,3.89485454 L3.97631488,0.139296592 C4.17083111,-0.0518420739 4.48263286,-0.0518571125 4.67716753,0.139262789 L25.6916134,20.7848311 C26.0855801,21.1718824 26.0911863,21.8050225 25.704135,22.1989893 C25.7000188,22.2031791 25.6958657,22.2073326 25.6916762,22.2114492 L4.67709797,42.8607841 C4.48259567,43.0519059 4.17082418,43.0519358 3.97628526,42.8608513 L0.154518591,39.1069479 C-0.0424848215,38.9134427 -0.0453206733,38.5968729 0.148184538,38.3998695 C0.150289256,38.3977268 0.152413239,38.395603 0.154556228,38.3934985 L16.9937789,21.8567812 C17.1908028,21.6632968 17.193672,21.3467273 17.0001876,21.1497035 C16.9980647,21.1475418 16.9959223,21.1453995 16.9937605,21.1432767 L0.15452076,4.60825197 C-0.0425130651,4.41477773 -0.0453986756,4.09820839 0.148075568,3.90117456 C0.150162624,3.89904911 0.152268631,3.89694235 0.154393339,3.89485454 Z"
                        fill="#FFFFFF"
                      ></path>
                    </g>
                  </svg>
                </span>
              </nuxt-link>
            </div>
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
          title: "Book your vehicle transportation online or by phone.",
          description:
            "It's simple to send a car using US Star Trucking! Using our online car shipping quotation tool, you just submit some necessary details of your shipment such as pickup and destination zip codes, trailer type, vehicle details and  shipping dates. Then one of our available agents will manually calculate the best competitive quotes and get back to you shortly via email and  phone call.  Then you can go ahead and compare our prices and services (we know you want to!) — we’re sure you’ll find our prices very competitive.",
        },
        {
          title: "We pick up your vehicle",
          description:
            "US Star Trucking experts will work with you to set up a pick-up time and date that works best for you. As a direct customer of our company, we do our best to work around your schedule and assign only trusted truckers for your shipment. When your trucker arrives, both of you will inspect your car together and sign a Bill of Lading. Then  the assigned trucker will take care of the rest. While your car is enjoying its journey, you can check in with your trucker directly  as often as  you wish to get updates.",
        },
        {
          title: "Receive your vehicle",
          description:
            "You will receive a short update from the driver some time before the drop off which should leave you with enough preparation time.  Then your assigned trucker will deliver your vehicle to your doorsteps (as we offer door-to-door service) or any other drop off location of your convenience. After a careful inspection to make sure everything looks good, you’ll simply sign the  Bill of landing to accept your delivery. That’s it!",
        },
      ],
    };
  },
};
</script>