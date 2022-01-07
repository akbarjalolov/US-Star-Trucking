<template>
  <div class="reviews pt-54 pb-54">
    <div class="container">
      <div class="row">
        <div class="col-12 mb-44" 
        data-aos="zoom-in"
         data-aos-once="true"
        data-aos-anchor-placement="center-bottom"
        data-aos-duration="600">
          <div class="d-flex align-items-center justify-content-between">
            <div>
              <h1 class="section-titles">
                <svg
                  width="39"
                  height="38"
                  viewBox="0 0 39 38"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M38.7265 13.9841C38.3941 12.9258 37.7299 12.0027 36.8322 11.3511C35.9345 10.6996 34.8509 10.3542 33.7418 10.3661H26.6409L24.4841 3.64393C24.1449 2.5858 23.4785 1.66272 22.5808 1.00781C21.6832 0.3529 20.6007 0 19.4896 0C18.3784 0 17.2959 0.3529 16.3983 1.00781C15.5007 1.66272 14.8342 2.5858 14.495 3.64393L12.3383 10.3661H5.23735C4.13174 10.3677 3.0549 10.7186 2.16064 11.3688C1.26638 12.019 0.600456 12.9351 0.257975 13.9863C-0.0845057 15.0375 -0.0860216 16.1701 0.253644 17.2223C0.59331 18.2744 1.25678 19.1923 2.1493 19.8449L7.92884 24.0706L5.73144 30.8757C5.37634 31.9312 5.37184 33.0731 5.71862 34.1314C6.0654 35.1896 6.74489 36.1074 7.65579 36.7479C8.55109 37.4091 9.63604 37.7632 10.749 37.7577C11.8619 37.7521 12.9433 37.3871 13.8319 36.7171L19.4896 32.553L25.1488 36.7122C26.0425 37.3695 27.1216 37.7266 28.231 37.732C29.3404 37.7374 30.4229 37.3909 31.323 36.7423C32.223 36.0936 32.8942 35.1763 33.24 34.1222C33.5859 33.0681 33.5885 31.9315 33.2477 30.8757L31.0503 24.0706L36.8363 19.8449C37.739 19.2005 38.4103 18.2826 38.7507 17.2271C39.0912 16.1715 39.0827 15.0344 38.7265 13.9841ZM34.9185 17.22L28.1833 22.143C27.9066 22.3448 27.7008 22.6289 27.5951 22.9546C27.4895 23.2803 27.4894 23.6311 27.5949 23.9569L30.1547 31.872C30.2843 32.2735 30.2832 32.7057 30.1516 33.1065C30.02 33.5073 29.7647 33.856 29.4224 34.1026C29.0802 34.3491 28.6685 34.4808 28.2467 34.4786C27.8248 34.4765 27.4146 34.3406 27.0748 34.0906L20.4517 29.2147C20.1728 29.0098 19.8357 28.8993 19.4896 28.8993C19.1434 28.8993 18.8063 29.0098 18.5274 29.2147L11.9043 34.0906C11.5648 34.344 11.1533 34.4827 10.7297 34.4865C10.306 34.4903 9.8921 34.3592 9.54801 34.1119C9.20391 33.8647 8.94749 33.5144 8.81592 33.1116C8.68435 32.7089 8.68447 32.2747 8.81625 31.872L11.3842 23.9569C11.4897 23.6311 11.4896 23.2803 11.384 22.9546C11.2783 22.6289 11.0725 22.3448 10.7959 22.143L4.06064 17.22C3.72145 16.9717 3.46942 16.6225 3.34054 16.2223C3.21167 15.8222 3.21254 15.3915 3.34305 14.9919C3.47355 14.5923 3.72701 14.2441 4.06721 13.9971C4.40741 13.7502 4.81696 13.617 5.23735 13.6167H13.5264C13.8705 13.6167 14.2057 13.5075 14.4837 13.3048C14.7618 13.1021 14.9683 12.8164 15.0736 12.4888L17.5928 4.63699C17.7222 4.23519 17.9756 3.88479 18.3168 3.63621C18.6579 3.38763 19.0691 3.25371 19.4912 3.25371C19.9133 3.25371 20.3245 3.38763 20.6656 3.63621C21.0068 3.88479 21.2602 4.23519 21.3895 4.63699L23.9087 12.4888C24.014 12.8164 24.2206 13.1021 24.4986 13.3048C24.7767 13.5075 25.1119 13.6167 25.456 13.6167H33.745C34.1654 13.617 34.575 13.7502 34.9152 13.9971C35.2554 14.2441 35.5088 14.5923 35.6393 14.9919C35.7698 15.3915 35.7707 15.8222 35.6418 16.2223C35.513 16.6225 35.2609 16.9717 34.9217 17.22H34.9185Z"
                    fill="white"
                  />
                </svg>
                Reviews
              </h1>
            </div>
            <div class="prev-next-arrows">
              <svg
                @click="prew()"
                width="48"
                height="48"
                viewBox="0 0 48 48"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M21.6982 27.8409L18.1627 24.3841C17.9458 24.172 17.9458 23.828 18.1627 23.6159L21.6982 20.1591C21.9152 19.947 22.267 19.947 22.4839 20.1591C22.7009 20.3712 22.7009 20.7151 22.4839 20.9273L19.8968 23.4568L47.4444 23.4568C47.7513 23.4568 48 23.7 48 24C48 24.3 47.7513 24.5432 47.4444 24.5432L19.8968 24.5432L22.4839 27.0727C22.7009 27.2849 22.7009 27.6288 22.4839 27.8409C22.267 28.053 21.9152 28.053 21.6982 27.8409Z"
                  fill="white"
                  fill-opacity="0.4"
                />
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M20.5 5.11111C10.3288 5.11111 2.08333 13.568 2.08333 24C2.08333 34.432 10.3288 42.8889 20.5 42.8889C30.6712 42.8889 38.9167 34.432 38.9167 24C38.9167 13.568 30.6712 5.11111 20.5 5.11111ZM20.5 4C9.73045 4 1 12.9543 1 24C1 35.0457 9.73045 44 20.5 44C31.2696 44 40 35.0457 40 24C40 12.9543 31.2696 4 20.5 4Z"
                  fill="white"
                  fill-opacity="0.4"
                />
              </svg>
              <svg
                @click="next()"
                class="ml-12"
                style="transform: rotate(180deg)"
                width="48"
                height="48"
                viewBox="0 0 48 48"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M21.6982 27.8409L18.1627 24.3841C17.9458 24.172 17.9458 23.828 18.1627 23.6159L21.6982 20.1591C21.9152 19.947 22.267 19.947 22.4839 20.1591C22.7009 20.3712 22.7009 20.7151 22.4839 20.9273L19.8968 23.4568L47.4444 23.4568C47.7513 23.4568 48 23.7 48 24C48 24.3 47.7513 24.5432 47.4444 24.5432L19.8968 24.5432L22.4839 27.0727C22.7009 27.2849 22.7009 27.6288 22.4839 27.8409C22.267 28.053 21.9152 28.053 21.6982 27.8409Z"
                  fill="white"
                  fill-opacity="0.4"
                />
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M20.5 5.11111C10.3288 5.11111 2.08333 13.568 2.08333 24C2.08333 34.432 10.3288 42.8889 20.5 42.8889C30.6712 42.8889 38.9167 34.432 38.9167 24C38.9167 13.568 30.6712 5.11111 20.5 5.11111ZM20.5 4C9.73045 4 1 12.9543 1 24C1 35.0457 9.73045 44 20.5 44C31.2696 44 40 35.0457 40 24C40 12.9543 31.2696 4 20.5 4Z"
                  fill="white"
                  fill-opacity="0.4"
                />
              </svg>
            </div>
          </div>
        </div>
        <div class="col-12"  data-aos="zoom-in-up"
         data-aos-once="true"
        data-aos-anchor-placement="center-bottom"
        data-aos-duration="800">
          <div>
            <VueSlickCarousel
              class="reviews-slider"
              ref="reviews"
              v-bind="settings"
            >
              <div
                class="review-cards"
                v-for="(item, index) in reviews"
                :key="index"
              >
                <div class="d-flex align-items-center mb-12 rev-head">
                  <div>
                    <img :src="item.img" alt="" />
                  </div>
                  <div>
                    <h6>
                      {{ item.firstName }}
                    </h6>
                    <p>
                      {{ item.from }}
                    </p>
                  </div>
                </div>
                <div class="rev-body mb-16">
                  <h3 class="mb-8">
                    {{ item.title }}
                  </h3>
                  <h4>
                    {{ item.full }}
                  </h4>
                </div>
                <div
                  class="
                    rev-bottom
                    d-flex
                    align-items-center
                    justify-content-between
                  "
                >
                  <div>
                    <h5>
                      {{ item.rating }}
                    </h5>
                    <svg
                      v-for="(stars, index) in item.stars"
                      :key="index"
                      width="14"
                      height="14"
                      viewBox="0 0 14 14"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M2.5918 7.56085L3.31581 8.08962L3.60784 8.3029L3.49672 8.64704L2.7518 10.954L2.74992 10.9598L2.74988 10.9598C2.66388 11.2154 2.66279 11.492 2.74678 11.7483C2.83077 12.0046 2.99534 12.2269 3.21596 12.382L3.22545 12.3887L3.22537 12.3888C3.44218 12.5489 3.70493 12.6347 3.97445 12.6334C4.24397 12.632 4.50584 12.5436 4.72105 12.3813L4.72567 12.3779L4.72569 12.3779L6.64366 10.9663L6.93982 10.7483L7.23613 10.9661L9.15465 12.376L9.15481 12.3761C9.37258 12.5363 9.63552 12.6233 9.90585 12.6246C10.1762 12.626 10.44 12.5415 10.6593 12.3835C10.8786 12.2254 11.0421 12.0019 11.1264 11.745C11.2107 11.4882 11.2113 11.2112 11.1283 10.954L10.3833 8.64704L10.2722 8.3029L10.5643 8.08962L12.5255 6.65722L2.5918 7.56085ZM2.5918 7.56085H2.59266L1.35673 6.65722C1.13925 6.49822 0.97758 6.27455 0.894814 6.01817C0.812047 5.76179 0.812416 5.48582 0.895869 5.22966C0.979322 4.97351 1.14159 4.75027 1.35949 4.59185C1.57731 4.43349 1.83959 4.34798 2.10889 4.34753C2.109 4.34753 2.1091 4.34753 2.1092 4.34753L4.51572 4.34753H4.8804L4.99182 4.00028L5.72297 1.72143L5.72301 1.72129C5.80566 1.46346 5.96805 1.23853 6.18678 1.07895L5.89209 0.675025L6.18678 1.07895C6.40551 0.919365 6.66928 0.833374 6.94003 0.833374C7.21079 0.833374 7.47455 0.919366 7.69329 1.07895L7.98798 0.675025L7.69329 1.07895C7.91202 1.23853 8.07441 1.46346 8.15706 1.7213L8.1571 1.72143L8.88825 4.00028L8.99966 4.34753H9.36435L11.7731 4.34753C11.7732 4.34753 11.7733 4.34753 11.7734 4.34753C12.0427 4.34798 12.305 4.43349 12.5228 4.59185C12.7407 4.75027 12.903 4.9735 12.9864 5.22966C13.0699 5.48582 13.0702 5.7618 12.9875 6.01817C12.9047 6.27447 12.7431 6.49807 12.5258 6.65707L2.5918 7.56085Z"
                        fill="#FFDF00"
                        stroke="#FDCC0D"
                      />
                    </svg>
                  </div>
                  <div>
                    <a :href="item.srcLink" target="_blank">
                      <img :src="item.source" alt="" />
                    </a>
                  </div>
                </div>
              </div>
            </VueSlickCarousel>
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
      settings: {
        infinite: false,
        speed: 500,
        slidesToShow: 3,
        slidesToScroll: 1,
        infinite: true,
        arrows: false,
        responsive: [
          {
            breakpoint: 1024,
            settings: {
              slidesToShow: 3,
              slidesToScroll: 3,
              infinite: true,
              dots: true,
            },
          },
          {
            breakpoint: 600,
            settings: {
              slidesToShow: 2,
              slidesToScroll: 2,
              initialSlide: 2,
            },
          },
          {
            breakpoint: 480,
            settings: {
              slidesToShow: 1,
              slidesToScroll: 1,
            },
          },
        ],
      },
      reviews: [
        {
          img: "images/profile-pic.png",
          firstName: "Emily Thorne",
          from: "Michigan",
          title: "Great service!",
          full: "Brad was very kind, and helped me with the process. I would recommend them because of his kindness and concern for the customer. He followed up with me and answered all of my questions- maintained communication with my husband and I. Thanks Brad !",
          rating: "5.0",
          stars: 5,
          source: "images/transport-reviews.png",
          srcLink: "google.com",
        },
        {
          img: "images/profile-pic.png",
          firstName: "Emily Thorne",
          from: "Michigan",
          title: "Great service!",
          full: "Brad was very kind, and helped me with the process. I would recommend them because of his kindness and concern for the customer. He followed up with me and answered all of my questions- maintained communication with my husband and I. Thanks Brad !",
          rating: "5.0",
          stars: 5,
          source: "images/transport-reviews.png",
          srcLink: "google.com",
        },
        {
          img: "images/profile-pic.png",
          firstName: "Emily Thorne",
          from: "Michigan",
          title: "Great service!",
          full: "Brad was very kind, and helped me with the process. I would recommend them because of his kindness and concern for the customer. He followed up with me and answered all of my questions- maintained communication with my husband and I. Thanks Brad !",
          rating: "5.0",
          stars: 5,
          source: "images/transport-reviews.png",
          srcLink: "google.com",
        },
        {
          img: "images/profile-pic.png",
          firstName: "Emily Thorne",
          from: "Michigan",
          title: "Great service!",
          full: "Brad was very kind, and helped me with the process. I would recommend them because of his kindness and concern for the customer. He followed up with me and answered all of my questions- maintained communication with my husband and I. Thanks Brad !",
          rating: "5.0",
          stars: 5,
          source: "images/transport-reviews.png",
          srcLink: "google.com",
        },
      ],
    };
  },

  methods: {
    next() {
      this.$refs.reviews.next();
    },
    prew() {
      this.$refs.reviews.prev();
    },
  },
};
</script>