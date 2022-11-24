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
  justify-content: space-between;
}
.first__frame {
  background-color: #8596aa;
  width: calc(100% / 3);
  height: 500px;
}
.second__frame {
  background-color: #2f5dab;
  width: calc(100% / 3);
  height: 500px;
}
.third__frame {
  background-color: #0f2d4a;
  width: calc(100% / 3);
  height: 500px;
}
</style>
