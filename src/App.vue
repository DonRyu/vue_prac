<template>
  <NavBar />
  <InfoBox />
  <ModalView/>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import InfoBox from "./components/InfoBox.vue";
import ModalView from "./components/ModalView.vue";

export default {
  name: "App",
  components: {
    NavBar,
    InfoBox,
    ModalView
  },
};
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
