<template>
  <div id="about" class="container">
    <img class="desk" src="../images/aboutus.svg" alt="about us" />
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
    <img class="mobile" src="../images/aboutus.svg" alt="about us" />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  min-height: 100vh;
  max-width: 100vw;
  img.desk {
    margin-top: 10%;
    margin-left: 15%;
  }
  .text {
    width: 25.5%;
    height: 10%;
    margin-left: 60%;
    margin-top: -30%;
    h1 {
      color: black;
      font-size: 5rem;
      font-weight: 700;
      line-height: 58px;
      margin-bottom: 5%;
    }
    p {
      color: black;
      font-size: 1.8rem;
      line-height: 28px;
      margin-bottom: 4%;
    }
    button {
      color: white;
      font-size: 1.8rem;
      font-weight: 600;
      padding: 1.5rem 2rem;
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
  img.mobile {
    display: none;
  }
}
@media screen and (max-width: 1440px) {
  .container {
    img.desk {
      margin-left: 4%;
    }
    .text {
      margin-left: 68%;
      margin-top: -40%;
    }
    button {
      margin-top: 5%;
    }
  }
}
@media screen and (max-width: 1024px) {
  .container {
    min-height: 70vh;
    img.desk {
      display: none;
    }
    img.mobile {
      display: block;
      margin: 15rem auto;
    }
    .text {
      width: 50%;
      margin: 10% 10%;
      h1 {
        font-size: 6rem;
      }
      p {
        line-height: 5rem;
      }
      button {
        margin-top: 3rem;
        padding: 3rem 5rem;
        font-size: 2rem;
      }
    }
  }
}

@media screen and (max-width: 768px) {
  .container {
    min-height: 70vh;
    img.desk {
      display: none;
    }
    img.mobile {
      display: block;
      margin: 15rem auto;
    }
    .text {
      width: 50%;
      margin: 10% 10%;
      h1 {
        font-size: 6rem;
      }
      p {
        line-height: 5rem;
      }
      button {
        margin-top: 3rem;
        padding: 3rem 5rem;
        font-size: 2rem;
      }
    }
  }
}

@media screen and (max-width: 375px) {
  .container {
    min-height: 70vh;
    img.desk {
      display: none;
    }
    img.mobile {
      display: block;
      margin: 15rem auto;
    }
    .text {
      width: 50%;
      margin: 5% 10%;
      h1 {
        font-size: 6rem;
      }
      p {
        line-height: 5rem;
      }
      button {
        margin-top: 3rem;
        padding: 3rem 5rem;
        font-size: 2rem;
      }
    }
  }
}
</style>
