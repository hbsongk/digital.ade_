<template>
  <footer>
    <a href="/contact" style="color: white">Contact</a>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=ABeeZee&display=swap");
* {
  position: relative;
  bottom: 0;
  font-family: "ABeeZee", sans-serif;
  font-size: 20px;
  font-style: bold;
  background-color: black;
}

footer {
  position: fixed;
  width: 100%;
  height: 100px;
}
</style>
