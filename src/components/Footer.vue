<template>
  <div id="footer" class="container">
    <footer>
      <div class="wrapper">
        <div class="desc">
          <h1>Devsforest</h1>
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the
            industry's standard dummy text ever since the 1500s
          </p>
          <div class="social">
            <button>
              <a href="https://www.facebook.com/"><i class="fab fa-facebook-f"></i></a>
            </button>
            <button>
              <a href="https://www.twitter.com/"><i class="fab fa-twitter"></i></a>
            </button>
            <button>
              <a href="https://www.instagram.com/"><i class="fab fa-instagram"></i></a>
            </button>
          </div>
        </div>
        <div class="lists">
          <h2>MENU</h2>
          <div class="list">
            <ul>
              <li><a href="#landing" v-smooth-scroll="{ duration: 1000 }">Home page</a></li>
              <li><a href="#about" v-smooth-scroll="{ duration: 1000 }">About Us</a></li>
              <li><a href="#tech" v-smooth-scroll="{ duration: 1000 }">Services</a></li>
              <li><a href="#contact" v-smooth-scroll="{ duration: 1000 }">Contact</a></li>
            </ul>
          </div>
        </div>

        <div class="lists">
          <h2>SERVICES</h2>
          <div class="list">
            <ul>
              <li>Web applications</li>
              <li>E-commerce</li>
              <li>Websites</li>
              <li>Vue.js</li>
            </ul>
          </div>
        </div>
        <div class="lists">
          <h2>CONTACT</h2>
          <div class="list">
            <ul>
              <li><i class="fas fa-phone-alt"></i> 123 456 789</li>
              <li><i class="far fa-envelope"></i> esample@index.com</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="line"></div>
      <p class="end">© Devsforest 2021. All rights reserved.</p>
    </footer>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  color: white;
  height: 70vh;
  max-width: 100vw;
  background: rgb(255, 255, 255);
  background-image: url('../images/footer.svg'),
    linear-gradient(
      180deg,
      rgba(255, 255, 255, 1) 0%,
      rgba(255, 255, 255, 1) 47%,
      rgba(28, 28, 28, 1) 50%,
      rgba(28, 28, 28, 1) 100%
    );
  background-repeat: no-repeat;
  footer {
    display: flex;
    flex-direction: column;
    padding-top: 12%;
    .wrapper {
      display: flex;
      width: 95%;
      justify-content: space-around;
      align-items: baseline;
      flex-wrap: wrap;
      .desc {
        width: 17%;
        h1 {
          font-size: 3.6rem;
          font-weight: 500;
          margin-bottom: 5%;
        }
        p {
          font-size: 1.8rem;
          font-weight: 400;
        }
        .social {
          display: flex;
          width: 70%;
          justify-content: space-around;
          margin-top: 10%;

          button {
            cursor: pointer;
            width: 50px;
            height: 50px;
            border: 1px solid white;
            background-color: transparent;
            text-align: center;
            border-radius: 50%;
            transition: 0.2s;

            i {
              color: white;
              font-size: 2rem;
            }
          }
          button:hover {
            background-color: white;
            i {
              color: #ffa47b;
            }
          }
        }
      }
      .lists {
        h2 {
          font-weight: 500;
          font-size: 2.4rem;
          line-height: 5rem;
        }
        .list {
          ul {
            display: flex;
            flex-direction: column;
            width: 150%;
            li {
              font-size: 1.8rem;
              list-style: none;
              height: 3rem;
              a {
                font-size: 1.8rem;
                text-decoration: none;
                color: white;
              }
            }
          }
        }
      }
    }
    .line {
      background-color: #ffffff;
      margin: 1.5rem auto;
      width: 90%;
      height: 2px;
    }
    .end {
      margin-top: 1%;
      font-weight: normal;
      color: white;
      text-align: center;
    }
  }
}
@media screen and (max-width: 375px) {
  .container {
    max-height: 40vh;
    footer {
      padding-top: 30%;
      .desc {
        display: none;
      }
    }
  }
}
</style>
