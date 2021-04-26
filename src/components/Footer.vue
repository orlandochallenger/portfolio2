<template>
    <div class="p-4 text-center ">
        <a href="https://github.com/orlandochallenger" target="_blank">
        <fa class="text-4xl mx-4" :icon="['fab','github']"/>
        </a>
        <a href="https://www.linkedin.com/in/orlando-challenger/" target="_blank">
        <fa class="text-4xl mx-4" :icon="['fab','linkedin']"/>
        </a>
    </div>
    <div class="pb-4 text-center">
        <span>&copy; {{new Date().getFullYear()}} Orlando Portfolio</span>
    </div>
    
</template>

<script>
export default {
    name: "Footer",

}
</script>

<style>

</style>