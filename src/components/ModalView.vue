<template>
  <div class="black-bg" v-if="isModal">
    <div class="white-bg">asd</div>
    <button>Close</button>
  </div>
</template>

<script>
export default {
  name: "ModalView",
  props:{
    isModal:Boolean
  }
};
</script>

<style scope>
.black-bg {
  width: 100%;
  height: 100%;
  background-color: rgb(0, 0, 0, 0.5);
  position: fixed;
  padding: 20px;
  top:0;
}

.white-bg {
  width: 100%;
  background-color: white;
  border-radius: 8px;
  padding: 20px;
}
</style>
