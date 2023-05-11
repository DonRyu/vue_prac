<template>
  <div
    v-for="(room, index) in roomList"
    :key="index"
    style="text-align: center; font-size: 40px"
  >
    <div style="font-weight: 500">{{ room.name }}</div>
    <div>{{ room.price }}</div>
    <button @click="increase(index)">Report</button> {{ report[index] }}
  </div>
</template>

<script>
export default {
  name: "InfoBox",
  data() {
    return {
      roomList: [
        { name: "a", price: 100, report: 0 },
        { name: "b", price: 200, report: 0 },
        { name: "c", price: 300, report: 0 },
      ],
      report: [0,0,0],
    };
  },
  methods: {
    increase(index) {
        this.report[index] +=1;
    },
  },
};
</script>

<style scope>

</style>
