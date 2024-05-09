<template>

    <body class="bg">
        <h1 class="ms-5 mt-3">Home</h1>
        <div class="containerdiv text-center mt-5 shadow-lg">
            <h2>Welcome to my web portfolio.</h2>
            <div>
                <img class="rounded-circle shadow-lg mt-3" alt="avatar" src="/assets/profilepic.png"
                    height="200" />
            </div>
            <div class="text-container mt-3">
                <p>My name is Tanner Green and I am a recent graduate of Algonquin College's Interactive Media
                    Design Program.
                    This website is a showcase of projects that display the skillset I developed during my studies. This site was coded
                    using Nuxt, Bootstrap, HTML, CSS, and JavaScript.
                    Please click one of the buttons below to navigate to a different page.
                </p>
                <NuxtLink to="/Resume"><button type="button" class="btn btn-primary">Resume</button></NuxtLink>
                <NuxtLink to="/design"><button type="button" class="btn btn-primary">Design/Video</button></NuxtLink>
                <NuxtLink to="/coding"><button type="button" class="btn btn-primary">Web Dev</button></NuxtLink>
                <NuxtLink to="/contact"><button type="button" class="btn btn-primary">Contact</button></NuxtLink>
            </div>
        </div>
                   
    </body>

    <footer></footer>
</template>

<script setup>


</script>

<style lang="css" scoped>

body {
    padding-top: 50px;
}

footer {
    height: 100px;
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

@media only screen and (max-width: 700px){
  
  .containerdiv {
      margin-left: 5%;
      margin-right: 5%;
  }


}
</style>