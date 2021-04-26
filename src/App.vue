<template>
  <LandingPage />
  <AboutUs />
  <Technologies />
</template>

<script>
import LandingPage from './components/LandingPage.vue';
import AboutUs from './components/AboutUs.vue';
import Technologies from './components/Technologies.vue';

export default {
  components: { LandingPage, AboutUs, Technologies },
};
</script>

<style lang="scss"></style>
