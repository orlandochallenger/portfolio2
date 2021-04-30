<template>
  <div>
    <NavBar />
    <router-view/>
    <Footer />
  </div>
</template>

<script>
import NavBar from "./components/NavBar"
import Footer from "./components/Footer"

export default {
  name: 'App',
  components: {
    NavBar,
    Footer
  }
}
</script>

<style scoped>
*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}
</style>