<template>
  <div class="landing">
    <Navbar />
    <h1>We love to create <br />software that <br />matters.</h1>
    <h2>We are developers with passion. We create <br />solutions tailored to your needs.</h2>
    <button>Read more</button>

    <img src="../images/landing-image.svg" alt="office" />
  </div>
</template>

<script>
import Navbar from '../layouts/Navbar.vue';

export default {
  components: { Navbar }
};
</script>

<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
}

div.landing {
  position: relative;
  min-width: 99vw;
  min-height: 100vh;
  background-image: url('../images/background.svg');
  //   background-size: cover;
  background-repeat: no-repeat;
}
// body {
//   background-image: url('../images/firstbg.svg'), url('../images/secondbg.svg'),
//     url('../images/thirdbg.svg'), url('../images/fourthbg.svg');
// }

h1 {
  line-height: 82px;
  font-weight: bold;
  font-size: 72px;
  position: absolute;
  left: 7rem;
  top: 20rem;
  text-shadow: 0px 1px 2px rgba(150, 150, 150, 1);
}
h2 {
  position: absolute;
  top: 37rem;
  left: 7rem;
  line-height: 38px;
  font-weight: normal;
}
button {
  position: absolute;
  top: 44rem;
  left: 7rem;
  background-color: white;
  color: black;
  border-radius: 5px;
  border: none;
  font-size: 18;
  font-weight: 600;
  padding: 15px 30px;
  text-shadow: 0px 1px 2px rgba(150, 150, 150, 1);
  box-shadow: 0px 1px 2px rgba(150, 150, 150, 1);
}
img {
  position: absolute;
  top: 11.7rem;
  left: 54rem;
}
</style>
