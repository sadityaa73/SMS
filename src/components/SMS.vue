<template>
  <div id="ContainerDiv">
    <HeaderComp />
    <MainContentContainer />
    <FooterComp />
  </div>
</template>
<script>
import HeaderComp from "../components/MainFile/HeaderComp.vue";
import FooterComp from "../components/MainFile/FooterComp.vue";
import MainContentContainer from "../components/MainFile/MainContentContainer.vue";
export default {
  name: "SMS",
  components: {
    HeaderComp,
    FooterComp,
    MainContentContainer,
  },
  data() {
    return {};
  },
};
</script>
<style scoped>
#ContainerDiv {
  display: flex;
  flex-direction: column;
}
</style>