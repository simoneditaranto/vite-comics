<script>
import AppNav from './components/AppNav.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppInfoLinks from './components/AppInfoLinks.vue';
import AppJumbo from './components/AppJumbo.vue';

export default {
  components: {
    AppNav,
    AppMain,
    AppFooter,
    AppInfoLinks,
    AppJumbo,
  }
}

</script>

<template>
  
  <AppNav></AppNav>

  <AppJumbo></AppJumbo>

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
