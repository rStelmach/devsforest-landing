<template>
  <div id="landing" class="landing">
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
  max-width: 100vw;
  min-height: 110vh;
  background-image: url('../images/background.svg');
  background-size: cover;
  background-repeat: no-repeat;
}

@media screen and (max-width: 375px) {
  .landing {
    min-height: 100vh;
    background-size: cover;
    background-position: center;
  }
}
</style>
