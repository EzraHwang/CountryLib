<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <SearchBox />
    <CountriesTable />
  </div>
</template>

<script>
import SearchBox from './components/SearchBox.vue'
import CountriesTable from './components/CountriesTable.vue'

export default {
  name: 'App',
  components: {
    SearchBox,
    CountriesTable
  }
}
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
