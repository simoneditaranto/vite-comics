<script>
import AppNav from './components/AppNav.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppInfoLinks from './components/AppInfoLinks.vue';

export default {
  components: {
    AppNav,
    AppMain,
    AppFooter,
    AppInfoLinks,
  }
}

</script>

<template>
  
  <AppNav></AppNav>

  <AppMain></AppMain>

  <AppFooter></AppFooter>

  <AppInfoLinks></AppInfoLinks>


</template>

<style>

*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
/* reset */

</style>
