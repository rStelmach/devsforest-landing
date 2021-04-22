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
* {
  margin: 0;
  padding: 0;
}
header {
  margin-left: 7%;
  margin-top: 2%;
  font-weight: 500;
  font-size: 30px;
}

div.landing {
  display: flex;
  flex-direction: column;
  min-width: 99vw;
  // max-width: 99vw;
  min-height: 100vh;
  background-image: url('../images/background.svg');
  background-repeat: no-repeat;
}
</style>
