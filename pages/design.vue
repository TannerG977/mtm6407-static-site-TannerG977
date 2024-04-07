<template>

    <body class="bg">
        <div>
            <h1 class="ms-5 mt-3">Design/Video</h1>
        </div>
        <div class="text-center mt-5">
            <div class="text-container mt-3">
                <p>This is a collection of Design/Video projects I've worked on during my time in IMD.</p>
            </div>
        </div>

        <div class="containerdiv mt-5 shadow-lg">
            <div class="text-container mt-3">
                <iframe class="shadow-lg mt-3" width="560" height="315" src="https://www.youtube.com/embed/sI_Y9308U5c?si=FDZ0A2N2mep5ePWg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
                <h2 class="mt-5">Promo Video For Inspect This Car</h2>
                <p>This was a promotional video that me and 5 other people worked on for the company, Inspect This Car. We were requested to film an educational video on the used car market, and how Inspect This Car improves the buying process. Me and one other person worked were tasked with doing all of the motion graphics and editing the footage. This is the final product.
                </p>
            </div>
        </div>

        <div class="containerdiv mt-5 shadow-lg">
            <div class="text-container mt-3">
                <iframe class="shadow-lg mt-3" width="560" height="315" src="https://www.youtube.com/embed/w6Vr4zZP9Ss?si=yIZO73KJRmNbJU7-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
                <h2 class="mt-5">DiefenBunker Documentary</h2>
                <p>This is a documentary that was a group collaboration between me and some classmates. The documentary is about the history of the DiefenBunker Museum in Carp Ontario.
                    For this production I designed and animated all of the motion graphics, and composed some of the music. The part i'm most proud of is the intro animation and music.
                </p>
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

iframe {
    width: 100%;
}
</style>