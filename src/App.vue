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

ul {
  list-style-type: none;
  display: flex;
}

ul li a {
  text-decoration: none;
  color: black;
  padding: 5px;
}

/* header */
header {
  background-color: white;
  height: 100px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 20px 0;
}

ul li a:hover {
  color: #0c7cec;
}
</style>