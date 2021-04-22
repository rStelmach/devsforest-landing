<template>
  <div class="landing">
    <header>Devsforest</header>
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
header {
  margin-left: 7%;
  margin-top: 2%;
  font-weight: 500;
  font-size: 30px;
}

.landing {
  display: flex;
  flex-direction: column;
  min-width: 100vw;
  min-height: 100vh;
  background-image: url('../images/background.svg');
  background-repeat: no-repeat;
}
</style>
