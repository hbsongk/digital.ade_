<template>
  <div id="app">
    <div id="nav">
      <nav>
        <main-header />
      </nav>
    </div>
    <router-view />
  </div>
</template>

<script>
import MainHeader from "@/components/MainHeader.vue";

export default {
  name: "App",
  components: {
    MainHeader,
  },
};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=ABeeZee&display=swap");
#app {
  font-family: "ABeeZee", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 10px;
  background-color: black;
}

nav a {
  font-weight: bold;
}
nav a.router-link {
  color: white;
}
nav a.router-link-exact-active {
  color: #42b983;
}
</style>
