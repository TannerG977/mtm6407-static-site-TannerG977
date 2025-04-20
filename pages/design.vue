<template>
    <body class="bg">
      <div class="container pt-12" data-aos="fade-up" data-aos-duration="1000">
        <h2 class="text-center text-3xl font-semibold bg-white p-6 rounded-3xl shadow-lg mb-10">
          A Collection of Video Projects I've Worked On
        </h2>
  
        <div class="row g-4">
          <div
            class="col-12 col-md-6 col-lg-4"
            v-for="(video, index) in videos"
            :key="index"
            data-aos="fade-up"
            data-aos-delay="index * 100"
          >
            <div class="rounded-4 shadow-lg bg-white overflow-hidden h-100 d-flex flex-column">
              <div class="vidcontainer">
                <iframe
                  :src="video.url"
                  class="rounded-top"
                  title="YouTube video player"
                  frameborder="0"
                  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                  referrerpolicy="strict-origin-when-cross-origin"
                  allowfullscreen
                ></iframe>
              </div>
              <div class="p-4 d-flex flex-column justify-content-between h-100">
                <h5 class="fw-bold mb-3">{{ video.title }}</h5>
                <p v-html="video.description" class="mb-0 text-sm"></p>
              </div>
            </div>
          </div>
        </div>
  
        <div class="text-center mt-5 mb-5 pb-5">
          <p class="text-lg text-white fw-medium">More Coming Soon!</p>
        </div>
      </div>
    </body>
  </template>
  
  <script setup>
  const videos = [
    {
      title: "Allercheck Connect (fake technology video)",
      url: "https://www.youtube.com/embed/69RVT2T5eCE?si=waEUsULkJkw1F3Va",
      description: `A futuristic allergy scanner concept produced as a final project with After Effects, Premiere Pro, and Mocha AE. I designed and animated the app UI.`,
    },
    {
      title: "Promo Video For Inspect This Car",
      url: "https://www.youtube.com/embed/VbvbbXO5Axc?si=ReowmCckGA0YW1Eb",
      description: `As team lead, I helped produce this promotional video for a used car inspection company, including all editing and motion graphics. It won 3rd at <a href="https://algonquincollege.my.site.com/myAC/EC_CommunityNewsDetail?id=a3hOG000000dQQsYAM" target="_blank" class="text-success text-decoration-underline">Algonquin's Applied Research Day</a>.`,
    },
    {
      title: "DiefenBunker Documentary",
      url: "https://www.youtube.com/embed/w6Vr4zZP9Ss?si=yIZO73KJRmNbJU7-",
      description: `A historical documentary on the Diefenbunker Museum. I created all motion graphics and composed the intro score.`,
    },
  ];
  </script>
  
  <style scoped>
  body {
    padding-top: 50px;
    font-family: 'Inter', sans-serif;
  }
  
  .bg {
    background-image: url("/assets/background.png");
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
    min-height: 100vh;
    width: 100vw;
    overflow-x: hidden;
  }

  .bg::before {
  content: "";
  position: fixed;
  inset: 0;
  background-image: inherit;
  background-size: cover;
  background-attachment: fixed;
  background-position: center;
  filter: blur(8px);
  z-index: -2;
}

.bg {
  position: relative;
  background-color: rgba(255, 255, 255, 0.6); /* subtle layer to soften */
  z-index: 0;
}
  
  .vidcontainer {
    position: relative;
    width: 100%;
    padding-top: 56.25%;
    background-color: #000;
  }
  
  iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: none;
  }
  
  .text-sm {
    font-size: 0.95rem;
    line-height: 1.5rem;
  }
  
  @media (max-width: 767px) {
    h2 {
      font-size: 1.5rem !important;
    }
  
    .p-4 {
      padding: 1.25rem !important;
    }
  
    .text-sm {
      font-size: 0.9rem;
    }
  }
  </style>
  