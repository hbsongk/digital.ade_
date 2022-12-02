<template>
  <div id="app">
    <div id="body__wrapper">
      <div id="nav">
        <nav>
          <main-header />
        </nav>
      </div>
      <router-view />
    </div>
    <main-footer style="position: relative; transform: translateY(-100%)" />
  </div>
</template>

<script>
import MainHeader from "@/components/MainHeader.vue";
import MainFooter from "@/components/MainFooter.vue";

export default {
  name: "App",
  components: {
    MainHeader,
    MainFooter,
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
#body__wrapper {
  position: relative;
  min-height: 100%;
  padding-bottom: 100px;
}
nav {
  padding: 10px;
  background-color: black;
}
</style>
