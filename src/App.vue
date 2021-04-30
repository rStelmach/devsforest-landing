<template>
  <LandingPage />
  <AboutUs />
  <Technologies />
  <ContactUs />
</template>

<script>
import LandingPage from './components/LandingPage.vue';
import AboutUs from './components/AboutUs.vue';
import Technologies from './components/Technologies.vue';
import ContactUs from './components/ContactUs.vue';

export default {
  components: { LandingPage, AboutUs, Technologies, ContactUs },
};
</script>

<style lang="scss"></style>
