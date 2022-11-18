<template>
  <div class="nav">
    <ul>
      <li><YdataVue /></li>
      <li><SourcedataVue /></li>
      <li><SourceAppVue /></li>
    </ul>
  </div>
</template>

<script>
import SourceAppVue from "./components/SourceApp.vue";
import SourcedataVue from "./components/Sourcedata.vue";
import YdataVue from "./components/Ydata.vue";
export default {
  name: "App",
  components: {
    SourceAppVue,
    SourcedataVue,
    YdataVue,
  },
};
</script>
<style>
.nav {
  margin: -7px;
  width: 105%;
  background-color: #f1f3f9;
  padding: 1px;
  height: 350px;
}
.nav ul {
  list-style: none;
  text-decoration: none;
  float: left;
}
</style>
