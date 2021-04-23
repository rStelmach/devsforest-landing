<template>
  <header>Devsforest</header>
  <nav>
    <ul>
      <li><a>Home</a></li>
      <li><a>Services</a></li>
      <li><a>About</a></li>
      <li><a>Blog</a></li>
      <li><a>Careers</a></li>
      <li><a>Contact Us</a></li>
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
      margin: 0 4%;
      list-style: none;
      cursor: pointer;

      a {
        font-size: 18px;
        text-decoration: none;
      }
    }
  }
}
</style>
