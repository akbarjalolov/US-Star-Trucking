<template>
  <div class="our-team pt-54 pb-54">
    <div class="container">
      <div class="row">
        <div class="col-12 mb-48">
          <div class="d-flex align-items-center">
           <svg width="27" height="40" viewBox="0 0 27 40" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M14.0601 21.6724L12.4129 31.5559L21.9667 18.3276H12.8529L14.5001 8.44406L4.9463 21.6724H14.0601ZM18.9729 1.95367C19.2635 0.209919 17.0024 -0.733597 15.9674 0.699526L0.319597 22.3657C-0.479203 23.4717 0.311086 25.0173 1.67541 25.0173H10.1116L7.94011 38.0463C7.64949 39.7901 9.91058 40.7336 10.9456 39.3005L26.5934 17.6343C27.3922 16.5283 26.6019 14.9827 25.2376 14.9827H16.8014L18.9729 1.95367Z" fill="white"/>
</svg>

            <h2 class="ml-18">Our team</h2>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-12 col-md-4 col-lg-3 col-sm-6"
        v-for="(item, index) in team" :key="index"
        >
          <div class="team-cards text-center mb-24">
            <img class="bg-effect" src="images/logo-background.svg" alt="">
            <div>
              <img :src="item.img" class="mb-16 ava" alt="">
            </div>
            <div>
              <h6 >{{item.name}}</h6>
              <p class="mb-48">{{item.position}}</p>
               <div class="socials">
            <a :href="item.insta" target="_blank">
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
            <a :href="item.fb" target="_blank">
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
         
            <a :href="item.twitter" target="_blank">
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
              :href="item.linkedln"
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
          </div>
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
      team: [
        {img: "images/akbar.png", name: "Frank Deamon", position: "Sales Agent", twitter: '', tg: '', fb: '', insta: '', linkedln: ''},
        {img: "images/akbar.png", name: "Frank Deamon", position: "Sales Agent", twitter: '', tg: '', fb: '', insta: '', linkedln: ''},
        {img: "images/akbar.png", name: "Frank Deamon", position: "Sales Agent", twitter: '', tg: '', fb: '', insta: '', linkedln: ''},
        {img: "images/akbar.png", name: "Frank Deamon", position: "Sales Agent", twitter: '', tg: '', fb: '', insta: '', linkedln: ''},
        {img: "images/akbar.png", name: "Frank Deamon", position: "Sales Agent", twitter: '', tg: '', fb: '', insta: '', linkedln: ''},
        {img: "images/akbar.png", name: "Frank Deamon", position: "Sales Agent", twitter: '', tg: '', fb: '', insta: '', linkedln: ''}
       
      ]
    }
  }
}
</script>