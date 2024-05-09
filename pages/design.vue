<template>

    <body class="bg">
        <div>
            <h1 class="ms-5 mt-3">Design/Video</h1>
        </div>
        <div class="text-center mt-5">
            <div class="text-container mt-3">
                <h5>This is a collection of Design/Video projects I've worked on.</h5>
            </div>
        </div>

        <div class="containerdiv mt-5 shadow-lg">
            <div class="text-container mt-3">
                <div class="vidcontainer">
                    <iframe class="shadow-lg mt-3 rounded" src="https://www.youtube.com/embed/69RVT2T5eCE?si=waEUsULkJkw1F3Va" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
                </div>
                <h2 class="mt-5">Allercheck Connect (fake technology video)</h2>
                <p>This is a video that me and two other classmates created as a final project. The goal of the project was to create a commercial for a technology that doesn't exist yet. Our idea was a device that could be stuck into food to scan for present allergens. We created this video using After Effects, Premier Pro, and Mocha AE. I was responsible for all of the app design and app animation present in the video. In addition to this I also helped with some other animations and some of the Mocha tracking.
                </p>
            </div>
        </div>

        <div class="containerdiv mt-5 shadow-lg">
            <div class="text-container mt-3">
                <div class="vidcontainer">
                    <iframe class="shadow-lg mt-3 rounded" src="https://www.youtube.com/embed/VbvbbXO5Axc?si=ReowmCckGA0YW1Eb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
                </div>
                <h2 class="mt-5">Promo Video For Inspect This Car</h2>
                <p>This is a promotional video that me and five of my classmates created for the company: Inspect This Car. We were requested to film and edit an educational video on the used car market. In addition to this the video also highlights how Inspect This Car's services enriches the process. Me and one other classmate were tasked with doing all of the motion graphics and editing the footage. Our final project was showcased at Algonquin College's Applied Research Day where we were awarded 3rd place out of 80 student projects from various different programs. The article can be found <a href="https://algonquincollege.my.site.com/myAC/EC_CommunityNewsDetail?id=a3hOG000000dQQsYAM&name=Students%20and%20faculty%20awarded%20for%20research%20projects%20at%20Applied%20Research%20Day">here</a>.
                </p>
            </div>
        </div>

        <div class="containerdiv mt-5 shadow-lg">
            <div class="text-container mt-3">
                <div class="vidcontainer">
                    <iframe class="shadow-lg mt-3 rounded" src="https://www.youtube.com/embed/w6Vr4zZP9Ss?si=yIZO73KJRmNbJU7-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
                </div>
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
    z-index: 1;
}

.portfolioimg {
    width: 100%;
}

.vidcontainer {
    position: relative;
    width: 100%;
    padding-top: 56.25%;
}

iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: 0;
    z-index: 1;
}

@media only screen and (max-width: 700px){
  
    .containerdiv {
        margin-left: 5%;
        margin-right: 5%;
    }


}

</style>