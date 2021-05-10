<template>
  <div id="tech" class="container">
    <section class="text">
      <h1>Technologies We Use</h1>
      <h2>
        Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's
        standard dummy text ever since the 1500s
      </h2>
    </section>
    <section class="box">
      <div>
        <img src="../images/html.svg" alt="HTML" />
        <h3>HTML</h3>
        <section class="desc">
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        </section>
      </div>
      <div>
        <img src="../images/vuejs.svg" alt="VueJS" />
        <h3>VueJS</h3>
        <section class="desc">
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        </section>
      </div>

      <div>
        <img src="../images/css.svg" alt="CSS" />
        <h3>CSS</h3>
        <section class="desc">
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        </section>
      </div>
      <div>
        <img src="../images/nodejs.svg" alt="NodeJS" />
        <h3>NodeJS</h3>
        <section class="desc">
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        </section>
      </div>
      <div>
        <img src="../images/js.svg" alt="JS" />
        <h3>JS</h3>
        <section class="desc">
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        </section>
      </div>

      <div>
        <img src="../images/react.svg" alt="React" />
        <h3>React</h3>
        <section class="desc">
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        </section>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  max-width: 100vw;
  min-height: 100vh;

  padding-top: 4%;
  background-color: #fff8ff;

  .text {
    max-width: 40%;
    text-align: center;
    margin: 0 auto;
    h1 {
      font-size: 5rem;
      font-weight: bold;
      color: black;
    }
    h2 {
      margin-top: 2%;
      font-size: 1.8rem;
      color: black;
    }
  }
  .box {
    display: flex;
    width: 61vw;
    height: 77vh;
    margin: 0 auto;
    margin-top: 1%;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    flex-wrap: wrap;

    div {
      display: flex;
      flex-direction: column;
      background-color: #ffffff;
      width: 30%;
      height: 45%;
      border: 1px solid #ffddff;
      border-radius: 20px;
      transition: 0.2s;

      img {
        display: block;
        margin: 0 auto;
        margin-top: 8%;
      }
      h3 {
        color: black;
        margin-top: 5%;
        text-align: center;
        font-size: 2.4rem;
        font-weight: 500;
      }

      .desc {
        width: 70%;
        height: 30%;
        margin: 0 auto;
        p {
          color: #5b5b5b;
          text-align: center;
          // margin-top: 5%;
          font-size: 1.8rem;
        }
      }
    }
    div:hover {
      box-shadow: 5px 24px 50px -10px rgba(135, 135, 135, 0.3);
    }

    // flex-basis: 1;
  }
}

@media screen and (max-width: 375px) {
  .container {
    .box {
      width: 95vw;
      div {
        height: 40%;
        img {
          margin-top: -5%;
          height: 60%;
          width: 60%;
        }
        h3 {
          margin-top: -20%;
        }
        p {
          margin-top: 5%;
        }
      }
    }
  }
}
</style>
