<template>
  <div>
    <div v-if="loading">
      <loader/>
    </div>
    <div class="wrapper" :class="loading ? '' : 'wrapper-transform'">
      <Header />
      <Nuxt />
      <Footer />
    </div>
  </div>
</template>

<script>
  import { mapState } from 'vuex'
import loader from '../components/loader.vue'

  export default {

  components: { loader },

  data() {
    return {
      loading: true
    }
  },

  mounted() {
    if ( this.loading == true) {
    setTimeout(() => {
      this.loading = false;
    }, 5000);
    }

  },
  }

</script>

<style lang="scss" scoped>
.wrapper {
  transform: translateY(100%);
  transition: 0.8s all;
  opacity: 0;
}

.wrapper-transform {
  transform: translateY(0%);
  opacity: 1;
}

.wrapper {
  transform: translateY(100%);
  transition: 0.8s all;
  opacity: 0;
}

.wrapper-transform {
  transform: translateY(0%);
  opacity: 1;
}



/* Track */
::-webkit-scrollbar-track {
  box-shadow: inset 0 0 5px grey; 
  border-radius: 10px;
}
 
/* Handle */
::-webkit-scrollbar-thumb {
  background: red; 
  border-radius: 10px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #b30000; 
}
</style>
