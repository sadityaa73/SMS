<template>
  <div id="TeacherdashBoard">
    <div id="infoBlock">
      <div id="blockContainer">
        <div id="block1">teacher</div>
        <div id="block2"></div>
        <div id="block3"></div>
      </div>
    </div>
    <div id="classTable_Notice">
      <div id="classTable"></div>
      <div id="Notice"></div>
    </div>
  </div>
</template>
<script>
export default {
  name: "teacherComp",
  data() {
    return {};
  },
};
</script>
<style scoped>
#infoBlock {
  display: flex;
  align-content: center;
  justify-content: space-between;
  border: 1px solid black;
  width: 926px;
  height: 24vh;
}
#blockContainer {
  display: flex;
  border: 1px solid red;
  width: 100%;
  justify-content: space-between;
  padding: 5px;
}
#block1 {
  display: flex;
  border: 1px solid black;
  height: 22vh;
  width: 200px;
  border-radius: 15px;
}
#block2 {
  display: flex;
  border: 1px solid black;
  height: 22vh;
  width: 200px;
  border-radius: 15px;
}
#block3 {
  display: flex;
  border: 1px solid black;
  height: 22vh;
  width: 200px;
  border-radius: 15px;
}
#classTable_Notice {
  display: flex;
  align-content: center;
  justify-content: space-between;
  border: 1px solid black;
  width: 926px;
  height: 55.5vh;
}
#classTable {
  display: flex;
  width: 60%;
  border: 1px solid blue;
  height: 51vh;
  margin: 24px;
}
#Notice {
  display: flex;
  width: 40%;
  border: 1px solid green;
  height: 51vh;
  margin: 24px;
}
</style>