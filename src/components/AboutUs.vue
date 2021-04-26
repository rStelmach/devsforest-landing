<template>
  <div class="container">
    <img src="../images/aboutus.svg" alt="about us" />
    <div class="text">
      <h1>About us</h1>
      <p>
        Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's
        standard dummy text ever since the 1500s, when an unknown printer took a galley of type.
      </p>
      <p>
        It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially
        unchanged.
      </p>
      <button>Read more</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  min-width: 100vw;
  min-height: 100vh;
  // background-color: green;

  img {
    margin-top: 10%;
    margin-left: 15%;
  }
  .text {
    width: 25.5%;
    height: 10%;
    margin-left: 60%;
    margin-top: -24%;
    h1 {
      color: black;
      font-size: 50px;
      font-weight: 700;
      line-height: 58px;
      margin-bottom: 5%;
    }
    p {
      color: black;
      font-size: 18px;
      line-height: 28px;
      margin-bottom: 4%;
    }
    button {
      color: white;
      font-size: 18px;
      font-weight: 600;
      padding: 1rem 2rem;
      border: none;
      border-radius: 5px;
      background: rgb(255, 154, 98);
      background: linear-gradient(
        90deg,
        rgba(255, 154, 98, 1) 0%,
        rgba(255, 114, 121, 1) 50%,
        rgba(255, 68, 147, 1) 100%
      );
      cursor: pointer;
    }
  }
}
</style>
