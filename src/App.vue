<script>
// import components
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
// export default
export default {
  name: 'Dc Comics',
  data() {
    return {
    }
  },
  components: { AppHeader, AppMain, AppFooter },
}
</script>

<template>
  <div class="container">
    <!-- header -->
    <AppHeader />

  </div>
</template>

<style>
/* reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* utilities */
.container {
  margin: 0 auto;
  max-width: 1200px;
}

/* generals */
img {
  max-width: 100%;
  height: auto;
}
</style>