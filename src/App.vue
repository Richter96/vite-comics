<script>
import SiteHeader from './components/siteHeader.vue';
import SiteMain from './components/SiteMain.vue';
import SiteFooter from './components/SiteFooter.vue';

export default {
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter,
  },
  data() {
    return {

    }
  },
}
</script>


<template>
  <SiteHeader></SiteHeader>
  <SiteMain></SiteMain>
  <SiteFooter></SiteFooter>
</template>




<style lang="scss">
// @use './node_modules/bootstrap/scss/bootstrap.scss';
@use './assets/scss/partials/variables' as *;

#app_header {
  text-align: center;
  background-color: #ffffff;

  img {
    padding: 1rem;
  }

  a {
    color: #0c7cec;
    text-decoration: none;
    padding: 0.5rem 1rem;
    border-bottom: 3px solid #0c7cec;

    &:not(.active) {
      border-bottom: none;
      color: black;

    }
  }



}




.banner {
  img {
    max-width: 50px;
  }

  .col {
    margin: 2rem 0;
    font-size: 0.7rem;
    display: flex;
    align-items: center;

    a {
      display: flex;
      align-items: center;
      width: 100%;

    }
  }
}
</style>