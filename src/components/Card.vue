<template>
    <div class="card" v-for="project in projects" :key="project.id">
        <img :src="project.image" style="width:100%;" :alt="project.title">
        <div class="container">
            <h2>{{ project.title }}</h2>
            <p>{{ project.desc }}</p>
            <button class="button"><a :href="project.url" target="_blank">View more</a></button>
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
                    image: "../assets/img/e_commerce.png",
                    title: "E-Commerce Site",
                    desc: "Created an e-commerce site with react and commerce.js",
                    url: "https://appleman-e-commerce.netlify.app/"
                },
                {
                    id: 2,
                    image: "../assets/img/employeeDirectory.png",
                    title: "Employee Directory",
                    desc: "Using HTML, CSS and JavaScript to create an employee directory by communicating with a third-party API",
                    url: "https://orlandochallenger.github.io/project-8/"
                },
                {
                    id: 3,
                    image: "../assets/img/WheelOfSucess.png",
                    title: "Game Show App",
                    desc: "In this project, I create a browser version of “Wheel of Success”, a word guessing game using HTML, CSS and JavaScript.",
                    url: "https://orlandochallenger.github.io/project-6/"
                },
                {
                    id: 4,
                    image: "../assets/img/gallery_mockup.png",
                    title: "Photo Gallery",
                    desc: "An Interactive Photo Gallery using HTML, CSS and JavaScript.",
                    url: "https://orlandochallenger.github.io/project-5/"
                },
                {
                    id: 5,
                    image: "../assets/img/Circle-UI-Kit.png",
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
a{
   text-decoration: none; 
   color: #000;
}

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

.button {
    display: inline-block;
    padding: 10px 25px;
    margin: 1rem;
    font-size: 24px;
    cursor: pointer;
    text-align: center;
    text-decoration: none;
    outline: none;
    color: #fff;
    background-color: #69cdfc;
    border: none;
    border-radius: 15px;
    box-shadow: 0 9px #999;
    transition-duration: 0.4s;
}

.button:hover {
  background-color: #a7d6ec; 
  color: rgb(18, 19, 20);
}

.button:active {
  background-color: #3e8e41;
  box-shadow: 0 5px #666;
  transform: translateY(4px);
}
</style>