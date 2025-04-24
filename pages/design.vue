<template>
   <body class="bg">
      <div class="container pt-12" data-aos="fade-up" data-aos-duration="1000">
        <div class="title">
            <h2 class="text-center hero-heading">
              Motion Design & Video Projects
            </h2>
        </div>
  
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
  
        
      </div>
    </body>
  </template>
  
  <script setup>
  const videos = [
    {
      title: "Deck Foot Anchor Facebook AD",
      url: "https://www.facebook.com/plugins/video.php?height=314&href=https%3A%2F%2Fwww.facebook.com%2Fdecksgo%2Fvideos%2F981598563791993%2F&show_text=false&width=560&t=0",
      description: `A high-performing Facebook ad I designed, shot, and edited for a digital campaign that reached over 500K views across all placements. The video opens with a Deck Foot Anchor logo, enhanced by light 3D work and rotoscoping to create an engaging, polished hook. This campaign was very successful and drove 20–30 daily email sign-ups.
`,
    },
    {
      title: "The Beast Of Gevaudan",
      url: "https://www.youtube.com/embed/YrDIA63sX4o?si=aFUGUSvgpCFS3Pfh",
      description: `This YouTube Short is a personal project that retells the legend of the Beast of Gévaudan. Using real footage as the base, I created each frame with a rotoscope technique, layering it with a dynamic "construction paper" texture for a handcrafted, surreal effect. Every element—from concept to final edit—was made by me.`,
    },
    {
      title: "Deck Renovation Series for DecksGo",
      url: "https://www.youtube.com/embed/videoseries?si=jzjvepY8AS7svBBk&amp;list=PLlGhyDiT_fi5OE-fXEBKCLVHS9V3wA_mV",
      description: `This playlist is a video series documenting the early stages of my work with Titan Building Products. I shot and edited extensive footage of CEO Richard Bergman as he renovated his personal deck, capturing detailed how-tos, product installs, and behind-the-scenes moments. The series showcases many hours of hands-on building, offering viewers both inspiration and insight.`,
    },
    {
      title: "Allercheck Connect (fake technology video)",
      url: "https://www.youtube.com/embed/69RVT2T5eCE?si=waEUsULkJkw1F3Va",
      description: `This concept video showcases a futuristic allergy scanner app. I designed and animated the entire UI, motion tracked the phone screen using Mocha AE, and overlaid the custom app animations to blend seamlessly with the live footage. Created as a final project using After Effects and Premiere Pro.`,
    },
    {
      title: "Promo Video For Inspect This Car",
      url: "https://www.youtube.com/embed/VbvbbXO5Axc?si=ReowmCckGA0YW1Eb",
      description: `During this project I was acting team lead over a group of 5 people. I was responsible for organizing all filming and took on a secondary role as motion graphics designer and editor. All motion graphics in the video were created by me. Me and my team were honoured to win 3rd place at <a href="https://www.algonquincollege.com/applied-research/category/applied-research/#:~:text=the%20project%20here.-,3rd%20Place,-%7C%20Inspect%20This" target="_blank" class="text-success text-decoration-underline">Algonquin's Applied Research Day</a>.`,
    },
    {
      title: "DiefenBunker Documentary",
      url: "https://www.youtube.com/embed/w6Vr4zZP9Ss?si=yIZO73KJRmNbJU7-",
      description: `This historical documentary explores the story of the Diefenbunker Museum. I assisted with the filming process and created the entire opening sequence using vector animation—one of my first ventures into the style. I also composed the original intro score and designed all motion graphics featured throughout the film.`,
    },
  ];
  </script>
  
  <style scoped>
  body {
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

  .title {
  background: #fff;
  border-radius: 16px;
  padding: 2rem;
  box-shadow: 0 20px 40px rgba(0,0,0,0.1);
  width: 80%;
  margin-left: auto;
  margin-right: auto;
  max-width: 960px;
  margin-top: 125px;
  margin-bottom: 20px;
}

.hero-heading {
  background: #c4e2bc;
  padding: 1.5rem;
  border-radius: 16px 16px 0 0;
  text-align: center;
  font-size: 1.75rem;
}

.swiper-container {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #fff;
  border-radius: 8px;
}

.swiper-pagination {
  bottom: 10px;
}

.swiper-button-next,
.swiper-button-prev {
  color: #fff;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 50%;
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

    .title {
      width: 100%;
    }
  }
  </style>
  