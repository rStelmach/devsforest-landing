<template>
  <LandingPage />
  <AboutUs />
  <Technologies />
  <ContactUs />
  <Footer />
</template>

<script>
import LandingPage from './components/LandingPage.vue';
import AboutUs from './components/AboutUs.vue';
import Technologies from './components/Technologies.vue';
import ContactUs from './components/ContactUs.vue';
import Footer from './components/Footer.vue';

export default {
  components: { LandingPage, AboutUs, Technologies, ContactUs, Footer },
};
</script>

<style lang="scss"></style>
