<template>
  <div class="container">
    <div class="text">
      <h1>We love to create <br />software that <br />matters.</h1>
      <h2>We are developers with passion. We create <br />solutions tailored to your needs.</h2>
      <button>Read more</button>
    </div>
    <img src="../images/landing-image.svg" alt="office" />
    <button class="responsive">Read more</button>
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
      line-height: 8.2rem;
      font-weight: bold;
      font-size: 7.2rem;
      text-shadow: 0px 1px 2px rgb(90, 90, 90);
    }
    h2 {
      margin-top: 5%;
      font-size: 2.8rem;
      line-height: 3.8rem;
      font-weight: normal;
    }
  }
  button {
    margin-top: 5%;
    background-color: white;
    color: black;
    border-radius: 5px;
    border: none;
    font-size: 1.8rem;
    font-weight: 600;
    padding: 15px 30px;
    text-shadow: 0px 2px 2px rgba(172, 171, 171, 0.7);
    box-shadow: 0px 1px 2px rgb(105, 105, 105);
    cursor: pointer;
  }
  img {
    margin-left: 7%;
    margin-top: 3%;
  }
  .responsive {
    display: none;
  }
}
@media screen and (max-width: 1440px) {
  .container {
    .text {
      margin-top: 15%;
    }
    img {
      margin-left: 4%;
      padding-top: 6%;
      height: auto;
      width: 47%;
    }
  }
}
@media screen and (max-width: 1024px) {
  .container {
    flex-direction: column;
    .text {
      h1 {
        margin-top: 0;
        line-height: 7rem;
        font-weight: bold;
        font-size: 7rem;
        text-shadow: 0px 1px 2px rgb(90, 90, 90);
      }
      h2 {
        margin-top: 3%;
        font-size: 2.8rem;
        font-weight: normal;
      }
      button {
        display: none;
      }
    }

    img {
      padding-top: 5%;
      height: auto;
      width: 80%;
    }
    .responsive {
      display: block;
      margin: 10% 45% 20% 15%;
      font-size: 3rem;
      padding: 2%;
    }
  }
}
@media screen and (max-width: 768px) {
  .container {
    flex-direction: column;
    // height: 80vh;
    .text {
      h1 {
        margin-top: 0;
        line-height: 7rem;
        font-weight: bold;
        font-size: 7rem;
        text-shadow: 0px 1px 2px rgb(90, 90, 90);
      }
      h2 {
        margin-top: 3%;
        font-size: 2.8rem;
        font-weight: normal;
      }
      button {
        display: none;
      }
    }

    img {
      padding-top: 5%;
      height: auto;
      width: 80%;
    }
    .responsive {
      display: block;
      margin: 10% 45% 20% 15%;
      font-size: 3rem;
      padding: 2%;
    }
  }
}
@media screen and (max-width: 375px) {
  .container {
    flex-direction: column;

    .text {
      h1 {
        line-height: 7rem;
        font-weight: bold;
        font-size: 7rem;
        text-shadow: 0px 1px 2px rgb(90, 90, 90);
      }
      h2 {
        margin-top: 3%;
        font-size: 2.8rem;
        font-weight: normal;
      }
      button {
        display: none;
      }
    }

    img {
      padding-top: 8%;
      height: auto;
      width: 80%;
    }
    .responsive {
      display: block;
      margin: 10% 40% 10% 15%;
      font-size: 3rem;
    }
  }
}
</style>
