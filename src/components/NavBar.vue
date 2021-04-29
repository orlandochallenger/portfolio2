<template>
    <nav class="fixed flex shadow-md z-50 justify-between items-center w-full p-4 bg-blue-300">
      <router-link to="/" class="flex flex-row text-2xl text-white">Orlando Challenger</router-link>
      <div>
        <router-link to="/" class="hover:bg-blue-400 mx-4 text-white">Home</router-link>
        <router-link to="/contact" class="hover:bg-blue-400 mx-4 text-white">Contact</router-link>
      </div>
    </nav>
</template>

<script>
export default {
    name: "NavBar"
}
</script>