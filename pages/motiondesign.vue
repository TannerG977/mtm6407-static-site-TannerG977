<template>
   <div class="bg">
      <div class="container">
        <div class="container">
        <div class="titlemd">
            <h2 class="hero-heading">Motion Graphics & Design Portfolio.</h2>
            <div class="intro-section2">
                <img class="avatar2" alt="avatar" src="/assets/profilepic.png"/>
                <div class="intro-text2">
                    <p>
                        Hi, I’m Tanner Green, a motion graphics designer and videographer with 3 years of experience in motion graphics and animation. This portfolio showcases a diverse range of work, including branding and motion graphics for both tech and creative industries. My expertise spans across 2D/3D animation, art direction, and storyboarding, with a strong focus on delivering impactful, visually engaging assets.

                        The projects featured here highlight my ability to create polished animations for various platforms, including social media, websites, and branding campaigns.

                        Feel free to explore and see how I bring creative concepts to life through motion design.
                    </p>
                </div>
            </div>
            <div class="webp-wrapper">
                <img src="/assets/leaf-animation.webp" alt="Animated WebP" class="webp-animation" />
                <img src="/assets/leaf-animation.webp" alt="Flipped Animated WebP" class="webp-animation flipped" />
            </div>
        </div>
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
    </div>
  </template>
  
  <script setup>
  const videos = [
    {
      title: "Deck Foot Anchor Facebook AD",
      url: "https://www.facebook.com/plugins/video.php?height=314&href=https%3A%2F%2Fwww.facebook.com%2Fdecksgo%2Fvideos%2F981598563791993%2F&show_text=false&width=560&t=0",
      description: `For this high-impact digital ad, I handled the full creative pipeline — from concept and shooting, to editing and motion design. The video opens with a dynamic Deck Foot Anchor logo animation, featuring subtle 3D modeling and light-based effects to create a sleek, professional hook. I incorporated rotoscoping and compositing to seamlessly integrate branding into live-action footage, enhancing visual polish and viewer retention.

This campaign reached over 500,000 views across placements and helped generate 20–30 email sign-ups per day, playing a key role in lead acquisition for the client. The piece was optimized for both paid and organic distribution, including cutdowns for Instagram and Facebook.

<br><br><strong>Tools used:</strong><br> After Effects, Blender, Premiere Pro, Mocha AE<br><br>
<strong>Skills showcased:</strong> <br>3D animation, compositing, logo reveal, storytelling, performance marketing visuals`,
    },
    {
      title: "The Beast Of Gevaudan",
      url: "https://www.youtube.com/embed/YrDIA63sX4o?si=aFUGUSvgpCFS3Pfh",
      description: `For this personal project, I handled the full creative pipeline — from concept and rotoscoping to final editing and animation. The video retells the eerie legend of the Beast of Gévaudan using real footage as a base, which I then traced frame-by-frame with rotoscoping. To achieve a handcrafted, surreal look, I layered the animation with a dynamic "construction paper" texture, giving the visuals a unique, tactile feel. Every element — from the creative concept to the final edit — was designed and executed by me.

This project allowed me to explore creative storytelling through a distinct visual style, which resonated with audiences for its unique aesthetic and engaging approach to an old legend.

<br><br><strong>Tools used:</strong><br> After Effects, Premiere Pro, Photoshop<br><br>
<strong>Skills showcased:</strong><br> Rotoscoping, texture mapping, frame-by-frame animation, storytelling, creative direction`,
    },
     {
      title: "Allercheck Connect (fake technology video)",
      url: "https://www.youtube.com/embed/69RVT2T5eCE?si=waEUsULkJkw1F3Va",
      description: `For this concept video, I created a futuristic allergy scanner app, handling every aspect from UI/UX design to animation and compositing. I designed the entire app interface and animated all the in-app interactions showcased throughout the video. Using Mocha AE, I motion tracked the phone screen in live-action footage, then composited the custom app animations to align perfectly with the device’s motion, resulting in a seamless, believable integration.

This was produced as a final project and demonstrates a full-stack motion design workflow — from concept and design to tracking, animation, and final edit.

<br><br><strong>Tools used:</strong><br> After Effects, Mocha AE, Premiere Pro, Illustrator<br><br>
<strong>Skills showcased:</strong><br> Motion tracking, UI/UX design, app animation, screen replacement, compositing, concept visualization`,
    },
    {
      title: "Xircls Meta Ads to WhatsApp Notifications (Instagram)",
      url: "https://www.youtube.com/embed/24feixuOJ4A",
      description: `For this Instagram animation, I created a short, engaging infographic to highlight Xircls' Meta Ads integration, which allows businesses to send WhatsApp messages directly to users' phones via Meta Ads. The video features a 2D animation that incorporates 3D planes and lighting effects to enhance the visual flow and depth of the information being presented. The combination of 2D and 3D elements helped create a dynamic, modern look that grabs attention while conveying complex features in a clear and concise manner.

This animation was optimized for Instagram, designed to hold viewers’ attention and drive engagement with the Xircls brand.

<br><br><strong>Tools used:</strong><br> After Effects, Illustrator<br><br>
<strong>Skills showcased:</strong><br> 2D/3D hybrid animation, infographic design, motion graphics, lighting effects, social media optimization`,
    },
    {
      title: "Xircls Whats App Broadcasts (Instagram)",
      url: "https://www.youtube.com/embed/vNJv0DdczDc",
      description: `For this Xircls promo video, I created a short-form animation to highlight their SMS messaging feature, which allows businesses to send announcements, updates, and promotional texts directly to their customers. The animation uses bold typography, iconography, and kinetic motion to clearly demonstrate how the feature works, while maintaining Xircls' brand voice and visual identity.

I used motion design to simplify technical concepts and guide the viewer through the feature’s benefits in a clean, high-impact way optimized for social media.

<br><br><strong>Tools used:</strong><br> After Effects, Illustrator<br><br>
<strong>Skills showcased:</strong><br> Kinetic typography, feature breakdown animation, branded motion graphics, social media optimization, product communication`,
    },
    {
      title: "TOPS Connectors Animated Logo",
      url: "https://www.youtube.com/embed/mnS0O8J_11A",
      description: `For this animated logo, I created a 2D motion sequence designed as both an intro and outro for TOPS Connectors' video content. The animation showcases one of the connector modules snapping into a bi-top configuration, which then seamlessly transforms into the letter “T” in the TOPS wordmark. This motion metaphor subtly reinforces the brand’s core value: modularity and expandability in pergola design.

The animation was designed to feel mechanical yet fluid, matching the product’s precision and flexibility while giving the logo a distinctive, branded personality.

<br><br><strong>Tools used:</strong><br> After Effects, Illustrator<br><br>
<strong>Skills showcased:</strong><br> Logo animation, 2D motion graphics, brand storytelling, transformation animation, visual identity development`,
    },
    {
      title: "Product Information Videos",
      url: "https://www.youtube.com/embed/videoseries?si=-LBZCaJob1p4HBwc&amp;list=PLlGhyDiT_fi7b55tTGNWOPr9lyudSE8Ez",
      description: `As a videographer and content creator at DecksGo, I filmed, edited, and produced a full suite of explainer videos for new product launches. This included both full-length walkthroughs and short-form cutdowns designed for high performance on social media platforms.

The project combined live-action video with layered 2D motion graphics, 3D animation, and motion tracking using Mocha AE to integrate product callouts and UI-style overlays directly into real footage. These dynamic visual elements helped clarify key features and improve viewer retention across formats.

The embedded YouTube playlist above showcases the complete collection of both long-form and short-form videos.

<br><br><strong>Tools used:</strong><br> After Effects, Mocha AE, Blender, Premiere Pro, Illustrator<br><br>
<strong>Skills showcased:</strong><br> Videography, 3D animation, motion tracking, motion design, product storytelling, social media optimization`,
    },
    {
      title: "Atlas Concrete Foot Anchor (Youtube Short)",
      url: "https://www.youtube.com/embed/FeAsdVVGM_c",
      description: `This short-form product video highlights the Atlas Concrete Anchor — a durable metal footing designed to secure posts in poured concrete. I created this piece to quickly communicate the product’s purpose and installation process in a visually engaging format.

The video combines 2D animation with motion tracking via Mocha AE to overlay graphics and text that follow the product in motion, enhancing clarity without interrupting flow. Designed for short-form platforms, the video strikes a balance between visual polish and quick-hitting information.

The video gained 1.6K views organically and stands out as one of the more popular entries in the brand’s short-form content library.

<br><br><strong>Tools used:</strong><br> After Effects, Mocha AE, Illustrator, Premiere Pro<br><br>
<strong>Skills showcased:</strong><br> Short-form storytelling, motion tracking, 2D animation, product education, visual clarity for performance marketing`,
    },
    {
      title: "Promo Video For Inspect This Car",
      url: "https://www.youtube.com/embed/VbvbbXO5Axc?si=ReowmCckGA0YW1Eb",
      description: `For this video project, I served as team lead over a group of five, organizing all filming logistics while also taking on a secondary role as motion graphics designer and editor. I was responsible for creating all the motion graphics featured in the final video, ensuring they were seamless and visually impactful.

The project was presented at Algonquin's Applied Research Day, where we were honoured to win 3rd place for our innovative work and successful collaboration.

<br><br><strong>Tools used:</strong><br> After Effects, Premiere Pro<br><br>
<strong>Skills showcased:</strong><br> Team leadership, motion graphics, video editing, project coordination, academic communication`,
    },
  ];

  </script>
  
  <style global>
  body {
    font-family: 'Inter', sans-serif;
  }

  .intro-text2 {
    font-size: 20px;
  }

  .avatar2{
    width: 250px;
  }

  .intro-section2 {
  text-align: center;
  font-size: 1.75rem;
  display: flex;
  gap: 2rem;
  margin-top: 2rem;
  align-items: center;
  justify-content: center;
  width: 100%;
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

  .titlemd {
  background: #fff;
  border-radius: 16px;
  padding: 2rem;
  box-shadow: 0 20px 40px rgba(0,0,0,0.1);
  width: 100%;
  margin-left: auto;
  margin-right: auto;
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
  