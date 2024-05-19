<template>
    <body class="bg">
        <div class="containerdiv mt-5 rounded-4 shadow-lg">
            <h2 class="h2background pt-4 pb-4 rounded-top-4 text-center">Welcome to my web portfolio.</h2>
            <div class="text-container mt-3">
              <div class="mt-5">
                <div>
                  <img class="avatar rounded-4 shadow-lg me-4" alt="avatar" src="/assets/profilepic.png"
                      height="175" />
                </div>
                <p>My name is Tanner Green and I am a recent graduate from the Algonquin College's Interactive Media Design Program. This website is a showcase of projects that display the skillset I have developed during my studies. I coded it using Nuxt, Bootstrap, HTML, CSS, and JavaScript. Click one of the buttons below to navigate to a different page.
                </p>
              </div>
                <div class="text-center mt-5 mb-3">
                  <NuxtLink to="/Resume"><button type="button" class="button-18 m-1">Resume &#9777;</button></NuxtLink>
                  <NuxtLink to="/design"><button type="button" class="button-18 m-1">Design/Video &#9658;</button></NuxtLink>
                  <NuxtLink to="/coding"><button type="button" class="button-18 m-1">Web Dev &#10092; &#10093;</button></NuxtLink>
                  <NuxtLink to="/contact"><button type="button" class="button-18 m-1">Contact &#9993;</button></NuxtLink>
                </div>
            </div>
        </div>

        
                   
    </body>

    <footer>
    </footer>
</template>

<script>
export default {
  head() {
    return {
      link: [
        { rel: 'preconnect', href: 'https://fonts.googleapis.com' },
        { rel: 'preconnect', href: 'https://fonts.gstatic.com', crossorigin: true },
        { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=Karla:ital,wght@0,200..800;1,200..800&display=swap' },
      ],
    }
  },
}
</script>

<style lang="css">

h1, h2, h3, h4, h5, h6 {
  font-weight: bold;
}

.avatar {
  float: left;
}

.h2background {
  background-color: #c4e2bc;
}

body {
    padding-top: 50px;
    font-family: "Karla", sans-serif;
    font-size: 110%;
}

footer {
    height: 50px;
}

.bg {
    background-image: url("/assets/background.png") !important;
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
    height: 100vh;
    width: auto;
}

.text-container {
    margin-left: 10%;
    margin-right: 10%;
}

.containerdiv {
    border: none !important;
    margin-left: 15%;
    margin-right: 15%;
    background-color: white;
    padding-bottom: 20px;
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

  .avatar {
    float: none;
    width: 100%;
    height: auto;
    margin-bottom: 40px;
  }

  p {
    text-align: center;
  }


}
</style>