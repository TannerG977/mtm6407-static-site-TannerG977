<template>

    <body class="bg">
        <div>
            <h1 class="ms-5 mt-3">Coding</h1>
        </div>
        <div class="text-center mt-5">
            <div class="text-container mt-3">
                <p>This is a collection of coding projects I've completed during my time doing website development.</p>
            </div>
        </div>

        <div class="containerdiv mt-5 shadow-lg">
            <div class="text-container mt-3">
                <div class="text-center">
                    <img class="portfolioimg shadow-lg mt-3 rounded" alt="contactbook" src="/assets/contactbook.png"/>
                </div>
                <h2 class="mt-5">Contact Book</h2>
                <p>This is a simple contact book web application I created. This website was created using Vue 3, Vite, Vue Router and Bootstrap. The site allows the user to create contacts and edit existing ones. In addition you can also search contacts, filter alphabetically by last name or first name and delete existing contacts. All contact data is saved to a user's local storage so when the page is reloaded their contacts remain on the page.
                </p>
                <div class="text-center">
                    <a href="https://contactbooktannerg977.netlify.app/"><button type="button" class="btn btn-primary">Visit Site</button></a>
                </div>
            </div>
        </div> 

        <div class="containerdiv mt-5 shadow-lg">
            <div class="text-container mt-3">
                <div class="text-center">
                    <img class="portfolioimg shadow-lg mt-3 rounded" alt="reviewsite" src="/assets/reviewsite.png"/>
                </div>
                <h2 class="mt-5">Movie Review Site</h2>
                <p>This is a movie review site created by me and three of my classmates as one of our final projects. We used Nuxt to build the front end and Strapi was used as a backend tool to populate the site with content. 
                    My job was to complete the initial setup to allow the team to work together using Nuxt and Strapi.
                    I setup both repositories and developed the code so the information from our Strapi API could be displayed on the site. 
                    In addition to this me and one other person were tasked with creating all of the site's functionality, while our other two members were responsible for styling the site. 
                    We also used a free version of Cloudinary in order to share media such as images between all members of the project. Due to us using the free version of Cloudinary, the reviews page may not load very fast so please be patient as it fetches our media bank.
                </p>
                <div class="text-center">
                    <a href="https://darntootinreviews.netlify.app/"><button type="button" class="btn btn-primary">Visit Site</button></a>
                </div>
            </div>
        </div> 

        <div class="containerdiv mt-5 shadow-lg">
            <div class="text-container mt-3">
                <div class="text-center">
                    <img class="portfolioimg shadow-lg mt-3 rounded" alt="quizsite" src="/assets/QuizSiteLogo.jpg"/>
                </div>
                <h2 class="mt-5">Quiz Site</h2>
                <p>This is a website I created that works as a functional quiz game. There are three different difficulty options and the site will track how many answers the user gets right or wrong until the reset button is hit.
                    It was coded using HTML, CSS, JavaScript, and uses QuizApi to retrieve the questions.
                </p>
                <div class="text-center">
                    <a href="https://tannerg977.github.io/mtm6302-capstone-TannerG977/"><button type="button" class="btn btn-primary">Visit Site</button></a>
                </div>
            </div>
        </div>  
        
        <div class="text-center mt-5 mb-5 pb-5">
            <div class="text-container mt-3">
                <p>More Coming Soon!</p>
            </div>
        </div>
    </body>
</template>

<script setup>


</script>

<style lang="css" scoped>

body {
    padding-top: 50px;
}

.bg {
    background-image: url("/assets/background.png") !important;
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
    height: 100vh;
    width: 100vw;
}

.text-container {
    margin-left: 10%;
    margin-right: 10%;
}

.btn-primary {
    background-color: #c4e2bc !important;
    color: black;
    margin-right: 12px !important;
    margin-top: 20px;
}

.btn-primary:hover {
    background-color: #688665 !important;
    color: white !important;
}

.containerdiv {
    border: solid #688665 10px;
    border-radius: 10px;
    margin-left: 15%;
    margin-right: 15%;
    background-color: white;
    padding-top: 20px;
    padding-bottom: 20px;
}

.portfolioimg {
    width: 100%;
}

@media only screen and (max-width: 700px){
  
  .containerdiv {
      margin-left: 5%;
      margin-right: 5%;
  }


}
</style>