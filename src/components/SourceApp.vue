<template>
  <div class="leftbar">
    <div class="left">
      <h1>数据应用</h1>
      <div class="leftcontainer">
        <div class="box">
          <img src="../assets/用户数量.png" />
          <p>{{ usenum }}</p>
        </div>
        <div class="leftbottom">用户数量</div>
      </div>
    </div>
    <div class="right">
      <div class="rightcontainer">
        <img src="../assets/车主数量.png" />
        <p>{{ carnum }}</p>
        <div class="rightbottom">车主数量</div>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  name: "SourceApp",
  setup() {
    let usenum = ref("58,123,326");
    let carnum = ref("600,000");
    return {
      carnum,
      usenum,
    };
  },
};
</script>

<style scoped>
.leftbar {
  width: 105%;
  height: 300px;
  background-color: #fdffff;
  float: left;
  margin-left: 180%;
  margin-top: -300px;
}
.left {
  float: left;
}
.box {
  border-right: 1px solid #eceef0;
  width: 190px;
}
.left h1 {
  margin: 13px 0 0 30px;
  font-size: 18px;
}
.leftcontainer {
  margin: 45px 0 0 80px;
}
.leftcontainer p {
  font-size: 40px;
  margin: 10px 0 0 -50px;
}

.right {
  float: right;
  margin-top: 77px;
  margin-left: 20px;
}
.rightcontainer {
  margin: 12px 20px 0 0px;
}
.rightcontainer img {
  margin-top: -8px;
}
.rightcontainer p {
  font-size: 40px;
  margin: 16px 0 0 -20px;
}
.leftbottom {
  font-size: 20px;
  margin: 20px 0 0 20px;
  color: #b2b4b6;
}
.rightbottom {
  font-size: 20px;
  margin: 20px 0 0 30px;
  color: #b2b4b6;
}
</style>
