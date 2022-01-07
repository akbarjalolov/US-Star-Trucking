<template>
  <div class="blog-slider-component pt-54 pb-54">
    <div class="container">
      <div class="row">
        <div
          class="col-12 mb-44"
          data-aos="zoom-in"
          data-aos-once="true"
          data-aos-anchor-placement="center-bottom"
          data-aos-duration="600"
        >
          <div class="d-flex align-items-center justify-content-between">
            <div>
              <h1 class="section-titles">
                <svg
                  width="39"
                  height="36"
                  viewBox="0 0 39 36"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M36.075 1.88933C35.1615 1.12547 34.091 0.572093 32.9395 0.268502C31.7881 -0.0350896 30.5839 -0.0814511 29.4125 0.132709L23.2017 1.26046C21.7678 1.52378 20.4641 2.2615 19.5 3.35508C18.5334 2.25961 17.2259 1.52172 15.7885 1.26046L9.5875 0.132709C8.41613 -0.0816385 7.21196 -0.0358845 6.06024 0.266732C4.90851 0.569349 3.83738 1.12143 2.92267 1.8839C2.00796 2.64636 1.27203 3.60057 0.766971 4.67898C0.261914 5.75739 7.93202e-05 6.93364 0 8.12446L0 25.6631C9.33657e-05 27.5656 0.667837 29.4078 1.88684 30.8685C3.10585 32.3293 4.7988 33.3159 6.67062 33.6565L16.8854 35.5138C18.6143 35.828 20.3857 35.828 22.1146 35.5138L32.3375 33.6565C34.2078 33.3142 35.8989 32.3268 37.1163 30.8663C38.3337 29.4057 39.0003 27.5645 39 25.6631V8.12446C39.0007 6.93406 38.739 5.75813 38.2334 4.68042C37.7279 3.60271 36.9909 2.64973 36.075 1.88933ZM17.875 32.3825C17.7385 32.363 17.602 32.3402 17.4655 32.3158L7.25237 30.4601C6.12912 30.2557 5.11321 29.6636 4.38179 28.787C3.65037 27.9103 3.24983 26.8048 3.25 25.6631V8.12446C3.25 6.83153 3.76361 5.59155 4.67785 4.67731C5.59209 3.76307 6.83207 3.24946 8.125 3.24946C8.41927 3.25016 8.71291 3.27681 9.0025 3.32908L15.21 4.46658C15.9569 4.60325 16.6323 4.9971 17.1191 5.57978C17.6059 6.16246 17.8734 6.89719 17.875 7.65646V32.3825ZM35.75 25.6631C35.7502 26.8048 35.3496 27.9103 34.6182 28.787C33.8868 29.6636 32.8709 30.2557 31.7476 30.4601L21.5345 32.3158C21.398 32.3402 21.2615 32.363 21.125 32.3825V7.65646C21.1249 6.89533 21.3919 6.1583 21.8795 5.57387C22.3671 4.98945 23.0444 4.5947 23.7932 4.45846L30.0024 3.32096C30.7055 3.19302 31.4282 3.22127 32.1193 3.40369C32.8103 3.58611 33.4528 3.91824 34.0012 4.37657C34.5496 4.83489 34.9905 5.4082 35.2927 6.05587C35.595 6.70354 35.7511 7.40975 35.75 8.12446V25.6631Z"
                    fill="white"
                  />
                </svg>

                Blog
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
      </div>
    </div>
    <div class="col-12"  data-aos="zoom-in-up"
         data-aos-once="true"
        data-aos-anchor-placement="center-bottom"
        data-aos-duration="800">
      <client-only placeholder="Loading...">
        <carousel-3d v-bind="settings" ref="blogSlides" class="blog-slides">
          <slide :index="index" v-for="(item, index) in blogInfo" :key="index">
            <nuxt-link :to="item.link">
              <h3>{{ item.title }}</h3>
              <p>
                {{ item.description }}
              </p>
              <div class="d-flex justify-content-between align-items-center">
                <div class="d-flex align-items-center">
                  <div>
                    <img :src="item.profile_pic" alt="" />
                  </div>
                  <div>
                    <h4>{{ item.name }}</h4>
                    <h5>{{ item.position }}</h5>
                  </div>
                </div>
                <div>
                  <svg
                    width="24"
                    height="18"
                    viewBox="0 0 24 18"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.5434 1.14147C15.4281 1.25578 15.3367 1.39177 15.2742 1.5416C15.2118 1.69144 15.1797 1.85216 15.1797 2.01447C15.1797 2.17679 15.2118 2.33751 15.2742 2.48734C15.3367 2.63718 15.4281 2.77317 15.5434 2.88747L21.1749 8.51896C21.2901 8.63326 21.3816 8.76926 21.444 8.91909C21.5064 9.06893 21.5386 9.22964 21.5386 9.39196C21.5386 9.55428 21.5064 9.71499 21.444 9.86483C21.3816 10.0147 21.2901 10.1507 21.1749 10.265L15.5434 15.8964C15.4281 16.0107 15.3367 16.1467 15.2743 16.2966C15.2118 16.4464 15.1797 16.6071 15.1797 16.7694C15.1797 16.9318 15.2118 17.0925 15.2743 17.2423C15.3367 17.3921 15.4281 17.5281 15.5434 17.6424C15.7738 17.8715 16.0854 18 16.4102 18C16.7351 18 17.0467 17.8715 17.2771 17.6424L22.9209 11.9987C23.6116 11.307 23.9996 10.3695 23.9996 9.39196C23.9996 8.41444 23.6116 7.47689 22.9209 6.78525L17.2771 1.14147C17.0467 0.912462 16.7351 0.783918 16.4102 0.783918C16.0854 0.783918 15.7738 0.912462 15.5434 1.14147Z"
                      fill="white"
                    />
                    <path
                      d="M7.95355 1.14147C7.8383 1.25578 7.74683 1.39177 7.68441 1.5416C7.62198 1.69144 7.58984 1.85216 7.58984 2.01447C7.58984 2.17679 7.62198 2.33751 7.68441 2.48734C7.74683 2.63718 7.8383 2.77317 7.95355 2.88747L13.585 8.51896C13.7003 8.63326 13.7917 8.76926 13.8542 8.91909C13.9166 9.06893 13.9487 9.22964 13.9487 9.39196C13.9487 9.55428 13.9166 9.71499 13.8542 9.86483C13.7917 10.0147 13.7003 10.1507 13.585 10.265L7.95355 15.8964C7.8383 16.0107 7.74683 16.1467 7.68441 16.2966C7.62198 16.4464 7.58984 16.6071 7.58984 16.7694C7.58984 16.9318 7.62198 17.0925 7.68441 17.2423C7.74683 17.3921 7.8383 17.5281 7.95355 17.6424C8.18393 17.8715 8.49557 18 8.8204 18C9.14524 18 9.45688 17.8715 9.68726 17.6424L15.331 11.9987C16.0218 11.307 16.4098 10.3695 16.4098 9.39196C16.4098 8.41444 16.0218 7.47689 15.331 6.78525L9.68726 1.14147C9.45688 0.912462 9.14524 0.783918 8.8204 0.783918C8.49557 0.783918 8.18393 0.912462 7.95355 1.14147Z"
                      fill="white"
                      fill-opacity="0.7"
                    />
                    <path
                      d="M0.363706 1.14147C0.24846 1.25578 0.156986 1.39177 0.0945621 1.5416C0.032138 1.69144 -7.05845e-07 1.85216 -6.9875e-07 2.01447C-6.91654e-07 2.17679 0.032138 2.33751 0.0945621 2.48734C0.156986 2.63718 0.24846 2.77317 0.363706 2.88747L5.99517 8.51896C6.11042 8.63326 6.20189 8.76926 6.26432 8.91909C6.32674 9.06893 6.35888 9.22964 6.35888 9.39196C6.35888 9.55428 6.32674 9.71499 6.26432 9.86483C6.20189 10.0147 6.11042 10.1507 5.99518 10.265L0.363707 15.8964C0.248461 16.0107 0.156987 16.1467 0.0945627 16.2966C0.0321387 16.4464 -6.08845e-08 16.6071 -5.37893e-08 16.7694C-4.66941e-08 16.9318 0.0321387 17.0925 0.0945628 17.2423C0.156987 17.3921 0.248461 17.5281 0.363707 17.6424C0.594084 17.8715 0.905723 18 1.23056 18C1.5554 18 1.86704 17.8715 2.09741 17.6424L7.74118 11.9987C8.43196 11.307 8.81996 10.3695 8.81996 9.39196C8.81996 8.41444 8.43196 7.47689 7.74118 6.78525L2.09741 1.14147C1.86703 0.912462 1.5554 0.783918 1.23056 0.783918C0.905722 0.783918 0.594083 0.912462 0.363706 1.14147Z"
                      fill="white"
                      fill-opacity="0.4"
                    />
                  </svg>
                </div>
              </div>
            </nuxt-link>
          </slide>
        </carousel-3d>
      </client-only>
    </div>
  </div>
</template>

<script>
import { Carousel3d, Slide } from "vue-carousel-3d";
export default {
  components: {
    Carousel3d,
    Slide,
  },

  data() {
    return {
      blogInfo: [
        {
          title: "Essentials in “Trucking”",
          description:
            "Brad was very kind, and helped me with the process. I would recommend them because of his kindness and concern for the customer. He followed up with me and answered all of my ques...",
          profile_pic: "/images/profile-pic-d.png",
          name: "Dean White",
          position: "Advisor/Agent",
          link: "asdas",
        },
        {
          title: "Essentials in “Trucking”",
          description:
            "Brad was very kind, and helped me with the process. I would recommend them because of his kindness and concern for the customer. He followed up with me and answered all of my ques...",
          profile_pic: "/images/profile-pic-d.png",
          name: "Dean White",
          position: "Advisor/Agent",
          link: "asdas",
        },{
          title: "Essentials in “Trucking”",
          description:
            "Brad was very kind, and helped me with the process. I would recommend them because of his kindness and concern for the customer. He followed up with me and answered all of my ques...",
          profile_pic: "/images/profile-pic-d.png",
          name: "Dean White",
          position: "Advisor/Agent",
          link: "asdas",
        },{
          title: "Essentials in “Trucking”",
          description:
            "Brad was very kind, and helped me with the process. I would recommend them because of his kindness and concern for the customer. He followed up with me and answered all of my ques...",
          profile_pic: "/images/profile-pic-d.png",
          name: "Dean White",
          position: "Advisor/Agent",
          link: "asdas",
        },{
          title: "Essentials in “Trucking”",
          description:
            "Brad was very kind, and helped me with the process. I would recommend them because of his kindness and concern for the customer. He followed up with me and answered all of my ques...",
          profile_pic: "/images/profile-pic-d.png",
          name: "Dean White",
          position: "Advisor/Agent",
          link: "asdas",
        },
      ],
      settings: {
        autoplay: true,
        autoplayTimeout: 5000,
        autoplayHoverPause: true,
        width: 587,
        height: 214,
        space: 200,
      },
    }
  },
  methods: {
    next() {
      this.$refs.blogSlides.goNext()
    },
    prew() {
            this.$refs.blogSlides.goPrev()
    }
  }
};
</script>