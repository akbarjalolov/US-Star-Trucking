<template>
  <footer class="footer pt-48 pb-24">
    <div class="container map">
      <div class="row">
        <div class="col-lg-3">
          <div class="pb-16">
              <nuxt-link class="logo" to="/">
            <img src="@/static/images/logo-footer.svg" alt="" />
              </nuxt-link>
          </div>
          <div>
            <a class="logo" href="https://www.fmcsa.dot.gov/">
            <img src="@/static/images/fmcsa-footer.svg" alt="" />
            </a>

          </div>
        </div>
        <div class="col-lg-4">
          <div class="d-flex justify-content-between">
            <div v-for="(item, index) in links" :key="index">
              <h5>
                {{ item.main_title }}
              </h5>
              <ul>
                <li v-for="(items, indexes) in item.childs" :key="indexes">
                  <nuxt-link :to="items.link">
                    {{ items.title }}
                  </nuxt-link>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="offset-lg-1 col-lg-4 form">
            <div class="relative mb-16">
              <h5 class="mb-20">Contact us</h5>
              <svg
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M17 3H7C4.23858 3 2 5.23858 2 8V16C2 18.7614 4.23858 21 7 21H16.9919L17.2087 20.9952C19.8687 20.8794 21.9901 18.6885 21.9939 16.0014L21.997 8.006L22 7.99797C22 5.23601 19.7607 2.99747 17 3ZM17.0009 5L17.1771 5.00494C18.6929 5.09145 19.907 6.30518 19.9949 7.8217L19.998 7.99949L19.9939 15.9995C19.9916 17.6556 18.6479 18.9985 16.991 19H7C5.34315 19 4 17.6569 4 16V8C4 6.34315 5.34315 5 7 5L17.0009 5Z"
                  fill="white"
                />
                <g opacity="0.5">
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M7.29289 8.29289C7.65338 7.93241 8.22061 7.90468 8.6129 8.2097L8.70711 8.29289L9.87868 9.46447C11.0034 10.5892 12.799 10.6342 13.9773 9.59943L14.1213 9.46447L15.2929 8.29289C15.6834 7.90237 16.3166 7.90237 16.7071 8.29289C17.0676 8.65338 17.0953 9.22061 16.7903 9.6129L16.7071 9.70711L15.5355 10.8787C13.6421 12.7721 10.6078 12.8295 8.64525 11.0508L8.46447 10.8787L7.29289 9.70711C6.90237 9.31658 6.90237 8.68342 7.29289 8.29289Z"
                    fill="white"
                  />
                </g>
              </svg>
              <div class="d-flex">
              <el-input placeholder="Your Email" v-model="email"> </el-input>
              <button class="white-btn">SUBMIT</button>
              </div>
             
            </div>
          <h5 class="mt-20 mb-8">Follow us</h5>
          <div class="socials">
            <a href="https://www.instagram.com/usstartrucking" target="_blank">
              <svg
                width="36"
                height="36"
                viewBox="0 0 36 36"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <rect
                  width="36"
                  height="36"
                  rx="6"
                  fill="white"
                  fill-opacity="0.2"
                />
                <path
                  d="M21.375 9H14.625C11.5189 9 9 11.5189 9 14.625V21.375C9 24.4811 11.5189 27 14.625 27H21.375C24.4811 27 27 24.4811 27 21.375V14.625C27 11.5189 24.4811 9 21.375 9ZM25.3125 21.375C25.3125 23.5463 23.5463 25.3125 21.375 25.3125H14.625C12.4538 25.3125 10.6875 23.5463 10.6875 21.375V14.625C10.6875 12.4538 12.4538 10.6875 14.625 10.6875H21.375C23.5463 10.6875 25.3125 12.4538 25.3125 14.625V21.375Z"
                  fill="white"
                />
                <path
                  d="M18 13.5C15.5149 13.5 13.5 15.5149 13.5 18C13.5 20.4851 15.5149 22.5 18 22.5C20.4851 22.5 22.5 20.4851 22.5 18C22.5 15.5149 20.4851 13.5 18 13.5ZM18 20.8125C16.4497 20.8125 15.1875 19.5503 15.1875 18C15.1875 16.4486 16.4497 15.1875 18 15.1875C19.5503 15.1875 20.8125 16.4486 20.8125 18C20.8125 19.5503 19.5503 20.8125 18 20.8125Z"
                  fill="white"
                />
                <path
                  d="M22.8369 13.7632C23.1681 13.7632 23.4366 13.4947 23.4366 13.1636C23.4366 12.8324 23.1681 12.564 22.8369 12.564C22.5058 12.564 22.2373 12.8324 22.2373 13.1636C22.2373 13.4947 22.5058 13.7632 22.8369 13.7632Z"
                  fill="white"
                />
              </svg>
            </a>
            <a href="https://www.facebook.com/usstartrucking" target="_blank">
              <svg
                width="36"
                height="36"
                viewBox="0 0 36 36"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <rect
                  width="36"
                  height="36"
                  rx="6"
                  fill="white"
                  fill-opacity="0.2"
                />
                <path
                  d="M22.5 15.1875H19.125V12.9375C19.125 12.3165 19.629 11.8125 20.25 11.8125H21.375V9H19.125C17.2609 9 15.75 10.5109 15.75 12.375V15.1875H13.5V18H15.75V27H19.125V18H21.375L22.5 15.1875Z"
                  fill="white"
                />
              </svg>
            </a>
            <a href="" target="_blank">
              <svg
                width="36"
                height="36"
                viewBox="0 0 36 36"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <rect
                  width="36"
                  height="36"
                  rx="6"
                  fill="white"
                  fill-opacity="0.2"
                />
                <path
                  d="M27.8554 12.6997C27.6188 11.7495 26.9218 11.0011 26.0367 10.7471C24.4324 10.2856 17.9996 10.2856 17.9996 10.2856C17.9996 10.2856 11.5667 10.2856 9.96246 10.7471C9.07739 11.0011 8.38032 11.7495 8.14373 12.6997C7.71387 14.422 7.71387 18.0155 7.71387 18.0155C7.71387 18.0155 7.71387 21.609 8.14373 23.3313C8.38032 24.2816 9.07739 24.9988 9.96246 25.2527C11.5667 25.7142 17.9996 25.7142 17.9996 25.7142C17.9996 25.7142 24.4324 25.7142 26.0367 25.2527C26.9218 24.9988 27.6188 24.2816 27.8554 23.3313C28.2853 21.609 28.2853 18.0155 28.2853 18.0155C28.2853 18.0155 28.2853 14.422 27.8554 12.6997ZM15.8957 21.2781V14.7529L21.2723 18.0156L15.8957 21.2781Z"
                  fill="white"
                />
              </svg>
            </a>
            <a href=" https://twitter.com/usstartrucking" target="_blank">
              <svg
                width="36"
                height="36"
                viewBox="0 0 36 36"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <rect
                  width="36"
                  height="36"
                  rx="6"
                  fill="white"
                  fill-opacity="0.2"
                />
                <path
                  d="M27 12.2319C26.3306 12.5255 25.6174 12.7201 24.8737 12.8146C25.6387 12.3579 26.2226 11.6401 26.4971 10.775C25.7839 11.2002 24.9964 11.5006 24.1571 11.6682C23.4799 10.9471 22.5146 10.5005 21.4616 10.5005C19.4186 10.5005 17.7739 12.1587 17.7739 14.1916C17.7739 14.4841 17.7986 14.7654 17.8594 15.0331C14.7915 14.8835 12.0769 13.4131 10.2532 11.1732C9.93487 11.7256 9.74813 12.3579 9.74813 13.0385C9.74813 14.3165 10.4062 15.4494 11.3872 16.1052C10.7944 16.094 10.2127 15.9219 9.72 15.6507C9.72 15.662 9.72 15.6766 9.72 15.6912C9.72 17.4845 10.9991 18.974 12.6765 19.3171C12.3761 19.3992 12.0487 19.4386 11.709 19.4386C11.4727 19.4386 11.2342 19.4251 11.0104 19.3756C11.4885 20.837 12.8453 21.9114 14.4585 21.9462C13.203 22.9284 11.6089 23.5201 9.88313 23.5201C9.5805 23.5201 9.29025 23.5066 9 23.4695C10.6346 24.5236 12.5719 25.1255 14.661 25.1255C21.4515 25.1255 25.164 19.5005 25.164 14.6247C25.164 14.4616 25.1584 14.3041 25.1505 14.1477C25.8829 13.628 26.4982 12.9789 27 12.2319Z"
                  fill="white"
                />
              </svg>
            </a>
            <a
              href=" https://www.linkedin.com/company/usstartruckingllc"
              target="_blank"
            >
              <svg
                width="36"
                height="36"
                viewBox="0 0 36 36"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <rect
                  width="36"
                  height="36"
                  rx="6"
                  fill="white"
                  fill-opacity="0.2"
                />
                <path
                  d="M12.3424 28.2857H7.97101V14.5286H12.3424V28.2857ZM10.1567 12.6C8.74244 12.6 7.71387 11.5714 7.71387 10.1572C7.71387 8.74287 8.87101 7.71429 10.1567 7.71429C11.571 7.71429 12.5996 8.74287 12.5996 10.1572C12.5996 11.5714 11.571 12.6 10.1567 12.6ZM28.2853 28.2857H23.9139V20.8286C23.9139 18.6429 23.0139 18 21.7281 18C20.4424 18 19.1567 19.0286 19.1567 20.9571V28.2857H14.7853V14.5286H18.8996V16.4572C19.2853 15.5572 20.8281 14.1429 23.0139 14.1429C25.4567 14.1429 28.0282 15.5572 28.0282 19.8V28.2857H28.2853Z"
                  fill="white"
                />
              </svg>
            </a>
            <!-- TODO: linkedln should be added -->
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-12 footer-bottom pt-24 mt-60" style="border-top: 1px solid #30313B;">
          <div class="d-flex align-items-center justify-content-between">
            <p>
              © 2021 US Star Trucking. All rights reserved.
            </p>
            <div>
            <nuxt-link class="mr-20" to="">
              Privacy Policy
            </nuxt-link>
            <nuxt-link to="">
              Terms & Conditions
            </nuxt-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import { mapState } from "vuex";
export default {
  name: "Footer",
  data() {
    return {
      links: [
        {
          main_title: "Company",
          childs: [
            { title: "Licensing & Terms", link: "asdas" },
            { title: "Licensing & Terms", link: "asdas" },
            { title: "Licensing & Terms", link: "asdas" },
            { title: "Licensing & Terms", link: "asdas" },
           
          ],
        },
        {
          main_title: "Company",
          childs: [
            { title: "Licensing & Terms", link: "asdas" },
            { title: "Licensing & Terms", link: "asdas" },
            { title: "Licensing & Terms", link: "asdas" },
            { title: "Licensing & Terms", link: "asdas" },
           
          ],
        },
      ],
      email: "",
    };
  },
};
</script>

<style lang="scss" scoped></style>
