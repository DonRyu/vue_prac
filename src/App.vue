<template>
  <NavBar />
  <InfoBox />
  <ModalView :isModal="isModal" />
  <div style="text-align: center">
    <Button @click="modalBtn">On</Button>
  </div>
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
    ModalView,
  },
  data(){
    return{
      isModal:false
    }
  },
  methods:{
    modalBtn(){
      this.isModal = !this.isModal
    }
  }
};
</script>

<style>
body {
  margin: 0;
}
div {
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
