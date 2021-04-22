<template>
  <div class="landing">
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
  </div>
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
.landing {
  padding-top: 40px;
  padding-bottom: 40px;
}
nav {
  ul {
    display: flex;
    justify-content: flex-end;
    align-items: baseline;
    margin-right: 8rem;

    li:last-child {
      color: white;
      border: 1px solid white;
      border-radius: 5px;
      padding: 1rem 2rem;
      font-weight: 600;
    }

    li {
      margin: 0 3rem;
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
