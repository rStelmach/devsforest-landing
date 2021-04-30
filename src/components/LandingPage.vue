<template>
  <div class="landing">
    <Navbar />
    <Hero />
  </div>
</template>

<script>
import Navbar from '../layouts/Navbar.vue';
import Hero from './Hero.vue';

export default {
  components: { Navbar, Hero },
};
</script>

<style lang="scss" scoped>
.landing {
  color: white;
  display: flex;
  flex-direction: column;
  // min-width: 100vw;
  max-width: 100vw;
  min-height: 110vh;
  background-image: url('../images/background.svg');
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
