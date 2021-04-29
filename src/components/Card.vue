<template>
<div class="flex flex-wrap mx-4">
    <div class="max-w-md mx-auto bg-indigo-50 rounded-xl shadow-md overflow-hidden md:max-w-2xl my-6" v-for="project in projects" :key="project.id">
        <div class="md:flex m-4">
            <div >
                <img class="vacation-card-image" :alt="project.title" :src="project.src" style="width:100%;" />
            </div>
            <div class="p-8">
                <a class="block mt-1 text-lg leading-tight font-medium text-black hover:underline" :href="project.url" target="_blank">{{ project.title }}</a>
                <p class="mt-2 text-gray-500">{{ project.desc }}</p>
            </div>
        </div> 
    </div>
</div>
        
</template>

<script>
export default {
    name: "Card",
    data() {
        return{
            projects: [
                {
                    id: 1,
                    src: require("../assets/img/e_commerce.png"),
                    title: "E-Commerce Site",
                    desc: "Created an e-commerce site with react and commerce.js.",
                    url: "https://appleman-e-commerce.netlify.app/"
                },
                {
                    id: 2,
                    src: require("../assets/img/todo.png"),
                    title: "Todo List Website",
                    desc: "Using node.js with express, mongoDB, and mongoose to create an todo list website.",
                    url: "https://aqueous-oasis-62492.herokuapp.com/"
                },
                {
                    id: 3,
                    src: require("../assets/img/gallery_mockup.png"),
                    title: "Photo Gallery",
                    desc: "An Interactive Photo Gallery using HTML, CSS and JavaScript.",
                    url: "https://orlandochallenger.github.io/project-5/"
                },
                {
                    id: 4,
                    src: require("../assets/img/employeeDirectory.png"),
                    title: "Employee Directory",
                    desc: "Using HTML, CSS and JavaScript to create an employee directory by communicating with a third-party API.",
                    url: "https://orlandochallenger.github.io/project-8/"
                },
                {
                    id: 5,
                    src: require("../assets/img/WheelOfSucess.png"),
                    title: "Game Show App",
                    desc: "In this project, I create a browser version of “Wheel of Success”, a word guessing game using HTML, CSS and JavaScript.",
                    url: "https://orlandochallenger.github.io/project-6/"
                },
                
            ]
        }
    } 
}
</script>
