<template>
  <div>
    <div v-if="loading">
      <loader/>
    </div>
    <div v-else class="wrapper">
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
    }, 3000);
    }

  },
  }

</script>

<style lang="scss" scoped>

</style>
