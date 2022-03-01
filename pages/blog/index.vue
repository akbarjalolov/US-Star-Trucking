<template>
  <div class="common blog mt-100">
    <div class="container pt-54 pb-54">
      <div class="row">
        <div class="col-12">
          <div class="d-flex align-items-center mb-48">
            <svg
              width="32"
              height="39"
              viewBox="0 0 32 39"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M0 7.09091C0 3.17471 3.17471 0 7.09091 0H21.881C23.7617 0 25.5653 0.747076 26.8951 2.07688L29.8322 5.01403C31.162 6.34384 31.9091 8.14743 31.9091 10.0281V31.9091C31.9091 35.8253 28.7344 39 24.8182 39H7.09091C3.17471 39 0 35.8253 0 31.9091V7.09091ZM28.3636 12.4091V31.9091C28.3636 33.8672 26.7763 35.4545 24.8182 35.4545H7.09091C5.13281 35.4545 3.54545 33.8672 3.54545 31.9091V7.09091C3.54545 5.13281 5.13281 3.54545 7.09091 3.54545H19.5V7.09091C19.5 10.0281 21.881 12.4091 24.8182 12.4091H28.3636ZM28.167 8.86364C27.9929 8.36301 27.7071 7.90295 27.3252 7.52105L24.388 4.58389C24.0061 4.20199 23.5461 3.91621 23.0455 3.74212V7.09091C23.0455 8.06996 23.8391 8.86364 24.8182 8.86364H28.167Z"
                fill="white"
              />
              <path
                d="M10.6364 19.5C9.65732 19.5 8.86365 20.2937 8.86365 21.2727C8.86365 22.2518 9.65732 23.0455 10.6364 23.0455H21.2727C22.2518 23.0455 23.0455 22.2518 23.0455 21.2727C23.0455 20.2937 22.2518 19.5 21.2727 19.5H10.6364Z"
                fill="white"
              />
              <path
                d="M10.6364 26.5909C9.65732 26.5909 8.86365 27.3846 8.86365 28.3636C8.86365 29.3427 9.65732 30.1364 10.6364 30.1364H15.9546C16.9336 30.1364 17.7273 29.3427 17.7273 28.3636C17.7273 27.3846 16.9336 26.5909 15.9546 26.5909H10.6364Z"
                fill="white"
              />
            </svg>

            <h2 class="ml-18">Blog</h2>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-12 col-sm-6 col-lg-4"
        v-for="(item, index) in blog" :key="index"
        >
          <nuxt-link class="blog-cards mb-20" :to="`blog/${item.link}`">
            <div class="image" v-bind:style="{ backgroundImage: 'url(' + item.img + ')' }">

            </div>
            <div class="info">
            <img class="logo-bg" src="images/logo-background.svg" alt="">

              <div class="d-flex align-items-center mb-13">
                <span >
                  <svg
                  class="mr-4"
                    width="20"
                    height="20"
                    viewBox="0 0 20 20"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M9.99996 16.6667C13.6819 16.6667 16.6666 13.6819 16.6666 10C16.6666 6.3181 13.6819 3.33333 9.99996 3.33333C6.31806 3.33333 3.33329 6.3181 3.33329 10C3.33329 13.6819 6.31806 16.6667 9.99996 16.6667ZM9.99996 18.3333C14.6023 18.3333 18.3333 14.6024 18.3333 10C18.3333 5.39762 14.6023 1.66666 9.99996 1.66666C5.39759 1.66666 1.66663 5.39762 1.66663 10C1.66663 14.6024 5.39759 18.3333 9.99996 18.3333Z"
                      fill="#E7E5EA"
                    />
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M9.99996 5C10.4602 5 10.8333 5.3731 10.8333 5.83333V9.65482L12.6725 11.4941C12.998 11.8195 12.998 12.3472 12.6725 12.6726C12.3471 12.998 11.8195 12.998 11.494 12.6726L9.4107 10.5893C9.25442 10.433 9.16663 10.221 9.16663 10V5.83333C9.16663 5.3731 9.53972 5 9.99996 5Z"
                      fill="#E7E5EA"
                    />
                  </svg>

                  {{item.time}}
                </span>
                <svg
                class="mr-8 ml-8" 
                  width="4"
                  height="4"
                  viewBox="0 0 4 4"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="2" cy="2" r="2" fill="#E7E5EA" />
                </svg>

                <span >
                  <svg
                  class="mr-4"
                    width="20"
                    height="20"
                    viewBox="0 0 20 20"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M15.8333 4.99999H4.16663C3.70639 4.99999 3.33329 5.37309 3.33329 5.83333V15.8333C3.33329 16.2936 3.70639 16.6667 4.16663 16.6667H15.8333C16.2935 16.6667 16.6666 16.2936 16.6666 15.8333V5.83333C16.6666 5.37309 16.2935 4.99999 15.8333 4.99999ZM4.16663 3.33333C2.78591 3.33333 1.66663 4.45262 1.66663 5.83333V15.8333C1.66663 17.214 2.78591 18.3333 4.16663 18.3333H15.8333C17.214 18.3333 18.3333 17.214 18.3333 15.8333V5.83333C18.3333 4.45262 17.214 3.33333 15.8333 3.33333H4.16663Z"
                      fill="#E7E5EA"
                    />
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M8.33333 10C7.8731 10 7.5 10.3731 7.5 10.8333C7.5 11.2936 7.8731 11.6667 8.33333 11.6667H14.1667C14.6269 11.6667 15 11.2936 15 10.8333C15 10.3731 14.6269 10 14.1667 10H8.33333ZM5.83333 13.3333C5.3731 13.3333 5 13.7064 5 14.1667C5 14.6269 5.3731 15 5.83333 15H10.8333C11.2936 15 11.6667 14.6269 11.6667 14.1667C11.6667 13.7064 11.2936 13.3333 10.8333 13.3333H5.83333Z"
                      fill="#E7E5EA"
                    />
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M5.83333 1.66667C5.3731 1.66667 5 2.03977 5 2.50001V5.83334C5 6.29358 5.3731 6.66667 5.83333 6.66667C6.29357 6.66667 6.66667 6.29358 6.66667 5.83334V2.50001C6.66667 2.03977 6.29357 1.66667 5.83333 1.66667ZM14.1667 1.66667C13.7064 1.66667 13.3333 2.03977 13.3333 2.50001V5.83334C13.3333 6.29358 13.7064 6.66667 14.1667 6.66667C14.6269 6.66667 15 6.29358 15 5.83334V2.50001C15 2.03977 14.6269 1.66667 14.1667 1.66667Z"
                      fill="#E7E5EA"
                    />
                  </svg>

                 {{item.date}}
                </span>
              </div>
              <div>
                <h6 class="mb-12">{{item.title}}</h6>
                <p>
                  {{item.description}}
                </p>
              </div>
            </div>
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: "pages",
  data() {
    return {
      blog: [
        {
          img: "images/blog.png",
          title: "Shipping Car From California To Virginia",
          description:
            "Open car hauler shipping is the standard method to transfer vehicles in large numbers across cities or states. It’s affordable, cost-effective, secure, and of course, fully insured against all accidental damages. At US Star Trucking, we want to make the proce...",
          time: "5 min",
          date: "Feb 17, 2022",
          link: "shipping-car-from-california-to-virginia",
        },
        {
          img: "images/blog.png",
          title: "Shipping Car From California To Virginia",
          description:
            "Open car hauler shipping is the standard method to transfer vehicles in large numbers across cities or states. It’s affordable, cost-effective, secure, and of course, fully insured against all accidental damages. At US Star Trucking, we want to make the proce...",
          time: "5 min",
          date: "Feb 17, 2022",
          link: "shipping-car-from-california-to-virginia",
        },
        {
          img: "images/blog.png",
          title: "Shipping Car From California To Virginia",
          description:
            "Open car hauler shipping is the standard method to transfer vehicles in large numbers across cities or states. It’s affordable, cost-effective, secure, and of course, fully insured against all accidental damages. At US Star Trucking, we want to make the proce...",
          time: "5 min",
          date: "Feb 17, 2022",
          link: "shipping-car-from-california-to-virginia",
        },
        {
          img: "images/blog.png",
          title: "Shipping Car From California To Virginia",
          description:
            "Open car hauler shipping is the standard method to transfer vehicles in large numbers across cities or states. It’s affordable, cost-effective, secure, and of course, fully insured against all accidental damages. At US Star Trucking, we want to make the proce...",
          time: "5 min",
          date: "Feb 17, 2022",
          link: "shipping-car-from-california-to-virginia",
        },
        {
          img: "images/blog.png",
          title: "Shipping Car From California To Virginia",
          description:
            "Open car hauler shipping is the standard method to transfer vehicles in large numbers across cities or states. It’s affordable, cost-effective, secure, and of course, fully insured against all accidental damages. At US Star Trucking, we want to make the proce...",
          time: "5 min",
          date: "Feb 17, 2022",
          link: "shipping-car-from-california-to-virginia",
        },  
      ],
    };
  },
};
</script>