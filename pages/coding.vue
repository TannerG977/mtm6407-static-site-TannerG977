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
                    <img class="portfolioimg shadow-lg mt-3" alt="quizlogo" src="/assets/QuizSiteLogo.jpg"/>
                </div>
                <h2 class="mt-5">Quiz Site</h2>
                <p>This website was a project I worked on during my time at Algonquin College. It is a functional quiz site that will ask the user
                    questions about coding topics. There are three different difficulty options and the site will track how many the user answers right or wrong, until the reset button is hit.
                    It was coded using HTML, CSS, JavaScript, and used QuizApi to retrieve the questions.
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
</style>