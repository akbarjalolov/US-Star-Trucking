<template>
  <div>
    <!-- <div v-if="$fetchState.pending" class="preloader"></div>
    <div v-else-if="$fetchState.error" class="error">Something is wrong here!</div> -->
    <div class="wrapper">
      <Header style="background: #28293A;
    border-bottom: 1px solid #E7E5EA;" />
      <Nuxt />
      <Footer />
    </div>
  </div>
</template>

<script>
  import { mapState } from 'vuex'

  export default {}
</script>

<style lang="scss" scoped></style>
