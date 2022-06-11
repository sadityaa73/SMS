<template>
  <div id="header">
    <div class="imgContainer">
      <img src="" alt="" />
    </div>
    <div class="home">
      <img src="" alt="" />
    </div>
  </div>
</template>
<script>
export default {
  name: "HeaderComp",
  data() {
    return {};
  },
};
</script>
<style scoped>
#header {
  display: flex;
  justify-content: space-between;
  border: 1px solid black;
  height: 8vh;
}
.imgContainer {
  display: flex;
  border: 1px solid black;
  width: 232px;
}
.home {
  display: flex;
  border: 1px solid black;
  width: 200px;
}
</style>