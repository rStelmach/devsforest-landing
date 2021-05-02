<template>
  <header>Devsforest</header>
  <nav>
    <ul>
      <li><a href="#landing" v-smooth-scroll="{ duration: 1000 }">Home</a></li>
      <li><a href="#tech" v-smooth-scroll="{ duration: 1000 }">Services</a></li>
      <li><a href="#about" v-smooth-scroll="{ duration: 1000 }">About</a></li>
      <li><a href="#footer" v-smooth-scroll="{ duration: 1000 }">Socials</a></li>
      <li><a>Careers</a></li>
      <li><a href="#contact" v-smooth-scroll="{ duration: 1000 }">Contact Us</a></li>
    </ul>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
* {
  font-family: 'Poppins', sans-serif;
  margin: 0;
  padding: 0;
}
header {
  margin-left: 7%;
  margin-top: 2%;
  font-weight: 500;
  font-size: 30px;
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
        font-size: 18px;
        text-decoration: none;
      }
    }
  }
}
</style>
