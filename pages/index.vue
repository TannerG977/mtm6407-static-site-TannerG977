<template>

    <body class="bg">
        <div>
            <h1 class="ms-5 mt-3">Home</h1>
        </div>
        <div class="text-center mt-5">
            <h2>Welcome to my web portfolio.</h2>
            <div>
                <img class="rounded-circle shadow-lg mt-3" alt="avatar" src="/assets/profilepic.png"
                    height="200" />
            </div>
            <div class="text-container mt-3">
                <p>Hi, My name is Tanner Green and I am a recent graduate of Algonquin College's Interactive Media
                    Design Program.
                    This website is a showcase of some of the projects I worked on while studying. This site was coded
                    using Nuxt and Bootstrap.
                    Please click one of the buttons below to navigate to a different page.
                </p>
                <NuxtLink to="/Resume"><button type="button" class="btn btn-primary">Resume</button></NuxtLink>
                <button type="button" class="btn btn-primary">Coding</button>
                <button type="button" class="btn btn-primary">Design</button>
                <NuxtLink to="/contact"><button type="button" class="btn btn-primary">Contact</button></NuxtLink>
            </div>
        </div>
                   
    </body>
</template>

<script setup>


</script>

<style lang="css" scoped>
.bg {
    background-image: url("/assets/background.png") !important;
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
    height: 100vh;
    width: 100vw;
}

.text-container {
    margin-left: 20%;
    margin-right: 20%;
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
</style>