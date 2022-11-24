<template>
  <div class="frame">
    <div class="first__frame"></div>
    <div class="second__frame"></div>
    <div class="third__frame"></div>
  </div>
</template>

<script>
export default {
  name: "MainFrame",
};
</script>

<style scoped>
.frame {
  display: flex;
  width: 100%;
}
.first__frame {
  background-color: red;
  width: 33%;
  height: 1000px;
}
.second__frame {
  background-color: blue;
  width: 33%;
  height: 1000px;
}
.third__frame {
  background-color: white;
  width: 33%;
  height: 1000px;
}
</style>
