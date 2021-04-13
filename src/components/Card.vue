<template>
    
    <div class="card" v-for="project in projects" :key="project.id">
        <img :src="project.img" style="width:100%">
        <div class="container">
            <h2>{{ project.title }}</h2>
            <p>{{ project.desc }}</p>
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
                    img: "../assets/img/e_commerce.png",
                    title: "E-Commerce Site",
                    desc: "Created an e-commerce site with react and commerce.js",
                    url: "https://appleman-e-commerce.netlify.app/"
                },
                {
                    d: 2,
                    img: "../assets/img/employeeDirectory.png",
                    title: "Employee Directory",
                    desc: "Using HTML, CSS and JavaScript to create an employee directory by communicating with a third-party API",
                    url: "https://orlandochallenger.github.io/project-8/"
                },
                {
                    id: 3,
                    img: "../assets/img/WheelOfSucess.png",
                    title: "Game Show App",
                    desc: "In this project, I create a browser version of “Wheel of Success”, a word guessing game using HTML, CSS and JavaScript.",
                    url: "https://orlandochallenger.github.io/project-6/"
                },
                {
                    id: 4,
                    img: "../assets/img/gallery_mockup.png",
                    title: "Photo Gallery",
                    desc: "An Interactive Photo Gallery using HTML, CSS and JavaScript.",
                    url: "https://orlandochallenger.github.io/project-5/"
                },
                {
                    id: 5,
                    img: "../assets/img/Circle-UI-Kit.png",
                    title: "Web Style Guide",
                    desc: "Web Style Guide using HTML, CSS and Sass as an important tool in a modern Front End Web Developer’s toolbox.",
                    url: "https://orlandochallenger.github.io/project-4/"
                }
            ]
        }
    } 
}
</script>

<style>
.card {
  /* Add shadows to create the "card" effect */
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 40%;
  margin: 1rem;
  border-radius: 5px;
}

/* On mouse-over, add a deeper shadow */
.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

/* Add some padding inside the card container */
.container {
  padding: 2px 16px;
}
</style>