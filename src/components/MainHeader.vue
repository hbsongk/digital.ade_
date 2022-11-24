<template>
  <header>
    <a href="/" class="logo"
      ><img
        alt="Digital.ade_ logo"
        src="../assets/logo_digital.ade_.svg"
        width="250"
    /></a>
    <div class="wrapper__router">
      <router-link
        style="color: gray; font-size: 20px"
        v-for="{ to, name } in [
          { to: '/', name: 'HOME' },
          { to: '/gallery', name: 'GALLERY' },
          { to: '/videos', name: 'VIDEOS' },
          { to: '/portfolio', name: 'PORTFOLIO' },
          { to: '/contact', name: 'CONTACT' },
        ]"
        :key="name"
        :to="to"
      >
        {{ name }}
      </router-link>
    </div>
    <div class="dropdown">
      <b-dropdown id="dropdown-1" text="Menu" class="m-md-2">
        <b-dropdown-item>First Action</b-dropdown-item>
        <b-dropdown-item>Second Action</b-dropdown-item>
        <b-dropdown-item>Third Action</b-dropdown-item>
        <b-dropdown-divider></b-dropdown-divider>
        <b-dropdown-item active>Active action</b-dropdown-item>
        <b-dropdown-item disabled>Disabled action</b-dropdown-item>
      </b-dropdown>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=ABeeZee&display=swap");
header {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  font-family: "ABeeZee", sans-serif;
}
.wrapper__router {
  width: 600px;
  display: flex;
  justify-content: space-evenly;
}
router-link:hover {
  color: red;
}
.dropdown {
  display: "";
}
.dropdown:hover {
  background-color: black;
}
@media screen and (max-width: 768px) {
  .wrapper__router {
    display: none;
  }
}
@media screen and (min-width: 768px) {
  .dropdown {
    display: none;
  }
}
</style>
