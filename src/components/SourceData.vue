<template>
  <div class="sourcedata">
    <h1>数据资产</h1>
    <div class="content">
      <img src="../assets/数据资产.png" />
      <p>{{ datanum }}</p>
      <div class="bottom">数据资产(表)</div>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  name: "SourceData",
  setup() {
    let datanum = ref("1,326");
    return {
      datanum,
    };
  },
};
</script>

<style scoped>
.sourcedata {
  height: 300px;
  float: left;
  margin-top: -300px;
  margin-left: 95%;
  background-color: #fdffff;
}
h1 {
  margin: 30px 0 0 50px;
  font-size: 18px;
}
.content {
  margin: 50px 130px;
}
img {
  margin-top: -22px;
}
.content p {
  font-size: 40px;
  margin: 6px 0 0 0px;
}
.bottom {
  font-size: 20px;
  margin: 22px 0 0 0px;
  color: #b2b4b6;
}
</style>
