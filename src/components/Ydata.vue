<template>
  <div class="leftbar">
    <div class="left">
      <h1>接入源数据</h1>
      <div class="leftcontainer">
        <div class="box">
          <img src="../assets/接入系统数.png" />
          <p>{{ systemnum }}</p>
        </div>
        <div class="leftbottom">接入系统数</div>
      </div>
    </div>
    <div class="right">
      <div class="rightcontainer">
        <img src="../assets/接入表数量.png" />
        <p>{{ tablenum }}</p>
        <div class="rightbottom">接入表数量</div>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  name: "Ydata",
  setup() {
    let systemnum = ref(40);
    let tablenum = ref(516);
    return {
      systemnum,
      tablenum,
    };
  },
};
</script>

<style scoped>
.leftbar {
  width: 450px;
  height: 300px;
  background-color: #507fdc;
  float: left;
  color: #fdffff;
  margin-left: -30px;
  margin-top: 15px;
}
.left {
  float: left;
}
.box {
  width: 120px;
  border-right: 1px solid #6a9cf2;
}
.left h1 {
  margin: 24px 0 0 30px;
  color: #effeff;
  font-size: 18px;
}
.leftcontainer {
  margin: 44px 0 0 70px;
}
.leftcontainer p {
  font-size: 40px;
  margin: 10px 0 0 0px;
  color: #effeff;
}
.bottom {
  font-size: 20px;
  margin: 20px 0 0 -20px;
}
.right {
  float: right;
  margin-top: -239px;
  margin-left: 100px;
}
.rightcontainer {
  margin: 62px 50px 0 0px;
}
.rightcontainer p {
  font-size: 40px;
  margin: 6px 0 0 30px;
}
.leftbottom {
  font-size: 20px;
  margin: 25px 0 0 -20px;
}
.rightbottom {
  font-size: 20px;
  margin: 25px 0 0 20px;
}
</style>
