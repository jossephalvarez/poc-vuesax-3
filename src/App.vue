<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <card-item/>
  </div>
</template>

<script>
import CardItem from './components/CardItem'

export default {
  name: 'App',
  components: {
    CardItem
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
