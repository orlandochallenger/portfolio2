<template>
  <NavBar />
  <main>
    <Card />
  </main>
</template>

<script>
import Card from './components/Card.vue'
import NavBar from "./components/NavBar"

export default {
  name: 'App',
  components: {
    Card,
    NavBar
  }
}
</script>

<style>
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* color: #2c3e50; */
  margin-top: 60px;
}

</style>
