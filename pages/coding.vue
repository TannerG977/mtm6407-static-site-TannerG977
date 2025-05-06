<template>

    <div class="bg">

        <div class="firstcontainer mt-5 shadow-lg rounded-4" data-aos="fade-up" data-aos-duration="1000">
            <h5 class="h2background pt-4 pb-4 rounded-top-4 text-center">This is a collection of web development projects I've worked on.</h5>
            <div class="text-container mt-3">
                <div class="text-center">
                    <img class="portfolioimg shadow-lg mt-3 rounded" alt="contactbook" src="/assets/contactbook.png"/>
                </div>
                <h2 class="mt-5">Contact Book</h2>
                <p>This is a simple contact book, web application I created. The website was created using Vue 3, Vite, Vue Router and Bootstrap. The site allows the user to create contacts and edit existing ones. In addition, you can search contacts, filter alphabetically by last name or first name and delete existing contacts. All contact data is saved to a user's local storage so when the page is reloaded, contacts remain on the page.
                </p>
                <div class="text-center">
                    <a href="https://contactbooktannerg977.netlify.app/"><button type="button" class="button-18">Visit Site</button></a>
                </div>
            </div>
        </div> 

        <div class="containerdiv mt-5 shadow-lg rounded-4" data-aos="fade-up" data-aos-duration="1000">
            <div class="text-container mt-3">
                <div class="text-center">
                    <img class="portfolioimg shadow-lg mt-3 rounded" alt="reviewsite" src="/assets/reviewsite.png"/>
                </div>
                <h2 class="mt-5">Movie Review Site</h2>
                <p>This is a movie review site created by me and three of my classmates as one of our final projects. We used Nuxt to build the front end and Strapi was used as a backend tool to populate the site with content. My responsibility was to complete the initial setup to allow the team to work together using Nuxt and Strapi. I set up both repositories and developed the code, so the information from our Strapi API could be displayed on the site. In addition, me and one other person were tasked with creating all of the site's functionality, while our other two members were responsible for styling the site. We also used a free version of Cloudinary in order to share media such as images between all members of the project. Due to us using the free version of Cloudinary, the reviews page may not load very fast so please be patient as it fetches our media bank.
                </p>
                <div class="text-center">
                    <a href="https://darntootinreviews.netlify.app/"><button type="button" class="button-18">Visit Site</button></a>
                </div>
            </div>
        </div> 

        <div class="containerdiv mt-5 shadow-lg rounded-4" data-aos="fade-up" data-aos-duration="1000">
            <div class="text-container mt-3">
                <div class="text-center">
                    <img class="portfolioimg shadow-lg mt-3 rounded" alt="quizsite" src="/assets/QuizSiteLogo.jpg"/>
                </div>
                <h2 class="mt-5">Quiz Site</h2>
                <p>This is a creation that works as a functional quiz game. There are three different difficulty options and the site will track how many answers the user gets right or wrong until the reset button is hit. It was coded using HTML, CSS, JavaScript, and uses QuizApi to retrieve the questions.
                </p>
                <div class="text-center">
                    <a href="https://tannerg977.github.io/mtm6302-capstone-TannerG977/"><button type="button" class="button-18">Visit Site</button></a>
                </div>
            </div>
        </div>  
        
        <div class="text-center mt-5 mb-5 pb-5">
            <div class="text-container mt-3">
                <p>More Coming Soon!</p>
            </div>
        </div>
    </div>
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
    margin-left: 15%;
    margin-right: 15%;
    background-color: white;
    padding-top: 20px;
    padding-bottom: 20px;
}

.firstcontainer {
    margin-left: 15%;
    margin-right: 15%;
    background-color: white;
    padding-bottom: 20px;
    z-index: 1;
}

.portfolioimg {
    width: 100%;
}

.button-18 {
  align-items: center;
  background-color: #c4e2bc !important;
  border: 0;
  border-radius: 100px;
  box-sizing: border-box;
  color: black;
  cursor: pointer;
  display: inline-flex;
  font-size: 16px;
  font-weight: 600;
  justify-content: center;
  line-height: 20px;
  max-width: 480px;
  min-height: 40px;
  min-width: 0px;
  overflow: hidden;
  padding: 0px;
  padding-left: 20px;
  padding-right: 20px;
  text-align: center;
  touch-action: manipulation;
  transition: background-color 0.167s cubic-bezier(0.4, 0, 0.2, 1) 0s, box-shadow 0.167s cubic-bezier(0.4, 0, 0.2, 1) 0s, color 0.167s cubic-bezier(0.4, 0, 0.2, 1) 0s;
  user-select: none;
  -webkit-user-select: none;
  vertical-align: middle;
}

.button-18:hover { 
  background-color: #688665 !important;
  color: #ffffff;
}


@media only screen and (max-width: 700px){
  
  .containerdiv {
      margin-left: 5%;
      margin-right: 5%;
  }

  .firstcontainer {
    margin-left: 5%;
    margin-right: 5%;
  }


}
</style>