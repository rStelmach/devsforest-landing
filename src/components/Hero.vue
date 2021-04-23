<template>
  <div class="container">
    <div class="text">
      <h1>We love to create <br />software that <br />matters.</h1>
      <h2>We are developers with passion. We create <br />solutions tailored to your needs.</h2>
      <button>Read more</button>
    </div>
    <img src="../images/landing-image.svg" alt="office" />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  display: flex;

  .text {
    margin-left: 7%;
    margin-top: 10%;
    h1 {
      line-height: 82px;
      font-weight: bold;
      font-size: 72px;
      text-shadow: 0px 1px 2px rgb(90, 90, 90);
    }
    h2 {
      margin-top: 5%;
      line-height: 38px;
      font-weight: normal;
    }
    button {
      margin-top: 5%;
      background-color: white;
      color: black;
      border-radius: 5px;
      border: none;
      font-size: 18;
      font-weight: 600;
      padding: 15px 30px;
      text-shadow: 0px 2px 2px rgb(172, 171, 171);
      box-shadow: 0px 1px 2px rgb(105, 105, 105);
      cursor: pointer;
    }
  }
  img {
    margin-left: 7%;
    margin-top: 3%;
  }
}
</style>
