<script>
import AppNav from './components/AppNav.vue';
import AppMain from './components/AppMain.vue';
import AppIcons from './components/AppIcons.vue';
import AppFooter from './components/AppFooter.vue';
import AppInfoLinks from './components/AppInfoLinks.vue';

export default {
  components: {
    AppNav,
    AppMain,
    AppIcons,
    AppFooter,
    AppInfoLinks,
  }
}

</script>

<template>
  
  <AppNav></AppNav>

  <AppMain></AppMain>

  <AppIcons></AppIcons>

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
