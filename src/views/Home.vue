<template>
  <div>
    <Header />
    <main class="bg-blue-200">
      <Card />
    </main>
  </div>
</template>

<script>
// @ is an alias to /src
import Card from '@/components/Card.vue'
import Header from '../components/Header'

export default {
  name: 'Home',
  components: {
    Card,
    Header
  }
}
</script>
