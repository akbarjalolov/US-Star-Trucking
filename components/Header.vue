<template>
  <header ref="header">
    <div class="container">
      <div class="row ">
        <div class="col-12 d-flex align-items-center justify-content-between pt-35 pb-35">
        <div class="logo">
          <nuxt-link to="/">
            <img src="@/static/images/logo.svg" class="logo" alt="" />
          </nuxt-link>
        </div>
        <div class="links">
          <ul class="d-flex">
            <li
              class="pr-18 pl-18"
              v-for="(item, index) in headerLink"
              :key="index"
            >
              <nuxt-link :to="item.link">
                {{ item.text }}
              </nuxt-link>
            </li>
          </ul>
        </div>
        <div class="socials">
          <a href="https://www.instagram.com/usstartrucking" target="_blank">
           <svg
            width="28"
            height="28"
            viewBox="0 0 28 28"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect
              width="28"
              height="28"
              rx="6"
              fill="white"
              fill-opacity="0.2"
            />
            <path
              d="M16.625 7H11.375C8.95913 7 7 8.95913 7 11.375V16.625C7 19.0409 8.95913 21 11.375 21H16.625C19.0409 21 21 19.0409 21 16.625V11.375C21 8.95913 19.0409 7 16.625 7ZM19.6875 16.625C19.6875 18.3138 18.3138 19.6875 16.625 19.6875H11.375C9.68625 19.6875 8.3125 18.3138 8.3125 16.625V11.375C8.3125 9.68625 9.68625 8.3125 11.375 8.3125H16.625C18.3138 8.3125 19.6875 9.68625 19.6875 11.375V16.625Z"
              fill="white"
            />
            <path
              d="M14 10.5C12.0671 10.5 10.5 12.0671 10.5 14C10.5 15.9329 12.0671 17.5 14 17.5C15.9329 17.5 17.5 15.9329 17.5 14C17.5 12.0671 15.9329 10.5 14 10.5ZM14 16.1875C12.7943 16.1875 11.8125 15.2057 11.8125 14C11.8125 12.7934 12.7943 11.8125 14 11.8125C15.2057 11.8125 16.1875 12.7934 16.1875 14C16.1875 15.2057 15.2057 16.1875 14 16.1875Z"
              fill="white"
            />
            <path
              d="M17.7623 10.7047C18.0198 10.7047 18.2286 10.4959 18.2286 10.2383C18.2286 9.98074 18.0198 9.77194 17.7623 9.77194C17.5047 9.77194 17.2959 9.98074 17.2959 10.2383C17.2959 10.4959 17.5047 10.7047 17.7623 10.7047Z"
              fill="white"
            />
          </svg>
          </a>
           <a href="https://www.facebook.com/usstartrucking" target="_blank">
          <svg
            width="28"
            height="28"
            viewBox="0 0 28 28"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect
              width="28"
              height="28"
              rx="6"
              fill="white"
              fill-opacity="0.2"
            />
            <path
              d="M17.5 11.8125H14.875V10.0625C14.875 9.5795 15.267 9.1875 15.75 9.1875H16.625V7H14.875C13.4251 7 12.25 8.17513 12.25 9.625V11.8125H10.5V14H12.25V21H14.875V14H16.625L17.5 11.8125Z"
              fill="white"
            />
          </svg>
         </a>
          <!-- <a href="" target="_blank">
             <svg
            width="28"
            height="28"
            viewBox="0 0 28 28"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect
              width="28"
              height="28"
              rx="6"
              fill="white"
              fill-opacity="0.2"
            />
            <path
              d="M21.6657 9.87759C21.4817 9.13853 20.9395 8.55647 20.2511 8.35894C19.0033 8 14 8 14 8C14 8 8.99669 8 7.7489 8.35894C7.06052 8.5565 6.51835 9.13853 6.33434 9.87759C6 11.2172 6 14.0121 6 14.0121C6 14.0121 6 16.8071 6.33434 18.1467C6.51835 18.8857 7.06052 19.4435 7.7489 19.6411C8.99669 20 14 20 14 20C14 20 19.0033 20 20.2511 19.6411C20.9395 19.4435 21.4817 18.8857 21.6657 18.1467C22 16.8071 22 14.0121 22 14.0121C22 14.0121 22 11.2172 21.6657 9.87759ZM12.3636 16.5497V11.4745L16.5454 14.0122L12.3636 16.5497Z"
              fill="white"
            />
          </svg>
          </a> -->
          <a href=" https://twitter.com/usstartrucking" target="_blank">
            <svg
            width="28"
            height="28"
            viewBox="0 0 28 28"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect
              width="28"
              height="28"
              rx="6"
              fill="white"
              fill-opacity="0.2"
            />
            <path
              d="M21 9.51374C20.4794 9.74212 19.9246 9.89349 19.3462 9.96699C19.9412 9.61174 20.3954 9.05349 20.6089 8.38061C20.0541 8.71136 19.4416 8.94499 18.7889 9.07537C18.2621 8.51449 17.5114 8.16711 16.6924 8.16711C15.1034 8.16711 13.8241 9.45687 13.8241 11.038C13.8241 11.2655 13.8434 11.4842 13.8906 11.6925C11.5045 11.5761 9.39313 10.4325 7.97475 8.69036C7.72712 9.11999 7.58188 9.61174 7.58188 10.1411C7.58188 11.1351 8.09375 12.0162 8.85675 12.5264C8.39562 12.5176 7.94325 12.3837 7.56 12.1729C7.56 12.1816 7.56 12.193 7.56 12.2044C7.56 13.5991 8.55487 14.7576 9.8595 15.0245C9.62587 15.0884 9.37125 15.119 9.107 15.119C8.92325 15.119 8.73775 15.1085 8.56362 15.07C8.9355 16.2066 9.99075 17.0422 11.2455 17.0694C10.269 17.8332 9.02912 18.2935 7.68688 18.2935C7.4515 18.2935 7.22575 18.283 7 18.2541C8.27137 19.074 9.77813 19.5421 11.403 19.5421C16.6845 19.5421 19.572 15.1671 19.572 11.3749C19.572 11.248 19.5676 11.1255 19.5615 11.0039C20.1311 10.5996 20.6097 10.0947 21 9.51374Z"
              fill="white"
            />
          </svg>
          </a>
          <a href=" https://www.linkedin.com/company/usstartruckingllc" target="_blank">
           <svg width="28" height="28" viewBox="0 0 28 28" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect width="28" height="28" rx="6" fill="white" fill-opacity="0.2"/>
<path d="M9.60001 22H6.2V11.3H9.60001V22ZM7.9 9.8C6.8 9.8 6 9 6 7.9C6 6.8 6.9 6 7.9 6C9 6 9.8 6.8 9.8 7.9C9.8 9 9 9.8 7.9 9.8ZM22 22H18.6V16.2C18.6 14.5 17.9 14 16.9 14C15.9 14 14.9 14.8 14.9 16.3V22H11.5V11.3H14.7V12.8C15 12.1 16.2 11 17.9 11C19.8 11 21.8 12.1 21.8 15.4V22H22Z" fill="white"/>
</svg>

          </a>
          <!-- TODO: linkedln should be added -->
        </div>
        <div>
          <a  target="_blank" href="https://apps.msgplane.com/quote/usst?id=24bc1d17-a5e2-45a0-8d54-a87a9f532e88">
          <button class="dark-btn">GET A QUOTE</button>
          </a>
        </div>
      </div>
      </div>
    </div>
  </header>
</template>

<script>
import { mapState } from "vuex";
export default {
  name: "Header",
  data() {
    return {
      scrollTop: 0,
      heightDevice: 0,
      activeMenu: false,
      headerLink: [
        { link: "about", text: "About Us", exact: true },
        { link: "team", text: "Our Team" },
        { link: "who-uses-us", text: "Who Uses Us" },
        { link: "information-center", text: "Information Center" },
        { link: "contact", text: "Contacts" },
      ],
    };
  },
 created() {
    if (process.client) {
      // eslint-disable-next-line nuxt/no-globals-in-created
      this.heightDevice = window.innerHeight;
      // eslint-disable-next-line nuxt/no-globals-in-created
      window.addEventListener("scroll", this.handleScroll);
    }
  },

  methods: {
    handleScroll(event) {
      this.scrollTop = process.client ? window.pageYOffset : 0;

      if (this. scrollTop > 100) {
        this.$refs.header.classList.add('header-changed')
      } else {
        this.$refs.header.classList.remove('header-changed')
      }
    },

  }
};
</script>

<style lang="scss" scoped>
</style>
