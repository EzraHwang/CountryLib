<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <SearchBox />
    <CountriesTable />
  </div>
</template>

<script>
import SearchBox from "./components/SearchBox.vue";
import CountriesTable from "./components/CountriesTable.vue";

import Vue from "vue";
import axios from "axios";
import VueAxios from "vue-axios";

Vue.use(VueAxios, axios);

export default {
  name: "App",
  created() {
    Vue.axios.get("https://restcountries.eu/rest/v2/name/united").then((response) => {
      console.log(response.data);
    });
  },
  components: {
    SearchBox,
    CountriesTable,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
