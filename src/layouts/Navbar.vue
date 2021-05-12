<template>
  <header>Devsforest</header>
  <nav>
    <ul>
      <li><a href="#landing" v-smooth-scroll="{ duration: 1000 }">Home</a></li>
      <li><a href="#tech" v-smooth-scroll="{ duration: 1000 }">Services</a></li>
      <li><a href="#about" v-smooth-scroll="{ duration: 1000 }">About</a></li>
      <li><a href="#footer" v-smooth-scroll="{ duration: 1000 }">Socials</a></li>
      <li><a href="#contact" v-smooth-scroll="{ duration: 1000 }">Contact Us</a></li>
    </ul>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
header {
  margin-left: 7%;
  margin-top: 2%;
  font-weight: 500;
  font-size: 3rem;
}

nav {
  ul {
    margin-top: -3%;
    margin-left: 30%;
    display: flex;
    justify-content: flex-end;
    align-items: baseline;
    margin-right: 6%;

    li:last-child {
      color: white;
      border: 1px solid white;
      border-radius: 5px;
      padding: 1rem 2rem;
      font-weight: 600;
    }

    li {
      color: white;
      margin: 0 4%;
      list-style: none;
      cursor: pointer;

      a {
        color: white;
        font-size: 1.8rem;
        text-decoration: none;
      }
    }
  }
}
@media screen and (max-width: 1024px) {
  header {
    margin-left: 5%;
    font-size: 3rem;
  }
  nav {
    ul {
      margin-right: 2%;
      li:last-child {
        text-align: center;
        padding: 1rem 1rem;
        a {
          font-weight: 600;
        }
      }
    }
  }
}

@media screen and (max-width: 768px) {
  header {
    margin-left: 5%;
    font-size: 3rem;
  }
  nav {
    ul {
      margin-right: 2%;
      li:last-child {
        text-align: center;
        padding: 0.5rem 1rem;
        a {
          font-weight: 600;
        }
      }
    }
  }
}

@media screen and (max-width: 375px) {
  header {
    margin-left: 5%;
    font-size: 2rem;
  }
  nav {
    ul {
      margin-right: 2%;
      li:last-child {
        text-align: center;
        padding: 0.5rem 1rem;
        a {
          font-weight: 600;
        }
      }
    }
  }
}
</style>
