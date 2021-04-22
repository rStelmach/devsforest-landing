<template>
  <LandingPage />
  <header>Devsforest</header>
</template>

<script>
import LandingPage from './components/LandingPage.vue';

export default {
  components: { LandingPage }
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');
* {
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
}
body {
  color: white;

  // background-image: url('./images/background.svg');
  // background-size: cover;
  // background-repeat: no-repeat;
}

header {
  position: absolute;
  top: 2rem;
  left: 8rem;
  font-weight: 500;
  font-size: 30px;
}
</style>
