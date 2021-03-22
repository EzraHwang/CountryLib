<template>
  <div id="app">
    <Home/>
    <CountriesTable/>
  </div>
</template>

<script>
import Home from './components/Home.vue'
import CountriesTable from './components/CountriesTable.vue'

export default {
  name: "App",
  components: {
    Home,
    CountriesTable
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
