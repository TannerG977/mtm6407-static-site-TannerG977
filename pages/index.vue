<template>
  <div class="bg">
    <div class="containerdiv">
      <h2 class="hero-heading">Welcome to my web portfolio.</h2>
      <div class="intro-section">
        <img class="avatar" alt="avatar" src="/assets/profilepic.png" height="150" />
        <div class="intro-text">
          <p>
            My name is Tanner Green, and I am a web developer, videographer, and graphic designer. This site showcases projects that reflect the skills I’ve developed throughout my professional and academic career. I coded this portfolio from scratch using nuxt.js, html, css, javascript, and bootstrap. Feel free to explore using the buttons below.
          </p>
        </div>
        <div class="pagebtns">
            <NuxtLink to="/Resume" class="btncontainer"><button class="btn-main">Resume</button></NuxtLink>
            <NuxtLink to="/design" class="btncontainer"><button class="btn-main">Video</button></NuxtLink>
            <NuxtLink to="/webdev" class="btncontainer"><button class="btn-main">Web Dev</button></NuxtLink>
            <NuxtLink to="/contact" class="btncontainer"><button class="btn-main">Contact</button></NuxtLink>
          </div>
      </div>
      <div class="webp-wrapper">
        <img src="/assets/leaf-animation.webp" alt="Animated WebP" class="webp-animation" />
        <img src="/assets/leaf-animation.webp" alt="Flipped Animated WebP" class="webp-animation flipped" />
      </div>
    </div>

    <!-- Featured Projects Section -->
    <div class="featured-section containerdiv mt-5">
      <h2 class="hero-heading text-center mb-4">Featured Projects</h2>
      <div class="project-grid">
        <div class="row">
          <div class="col-12 col-md-4 mb-4">
            <div class="project-card" data-aos="zoom-in" data-aos-once="true">
              <img src="/assets/DFA-AD thumbnail.png" alt="thumbnail of the Deck foot anchor lead magent ad video" class="mb-2"/>
              <h4>Deck Foot Anchor Facebook AD</h4>
              <p>A high-performing Facebook ad I designed, shot, and edited. The campaign drove over 500K views and 20-30 daily email signups.</p>
              <button class="featurebtn" @click="openModal">Learn More</button>
            </div>
          </div>
          <div class="col-12 col-md-4 mb-4">
            <div class="project-card" data-aos="zoom-in" data-aos-delay="100" data-aos-once="true">
              <img src="#" alt="Project 2" />
              <h4>Coming Soon</h4>
              <p>This project is loading</p>
            </div>
          </div>
          <div class="col-12 col-md-4 mb-4">
            <div class="project-card" data-aos="zoom-in" data-aos-delay="100" data-aos-once="true">
              <img src="#" alt="Project 3" />
              <h4>Coming Soon</h4>
              <p>This project is loading.</p>
            </div>
          </div>
        </div>
      </div>
      </div>
    </div>

  <div class="modal" :class="{ 'show': showModal }">
    <span class="close" @click="closeModal">&times;</span>
    <DFAFBAD />
  </div>
</template>

<script>
import { ref } from 'vue'
import DFAFBAD from '/components/DFA-FB-AD.vue'

export default {
  components: {
    DFAFBAD
  },
  head() {
    return {
      link: [
        { rel: 'preconnect', href: 'https://fonts.googleapis.com' },
        { rel: 'preconnect', href: 'https://fonts.gstatic.com', crossorigin: true },
        { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=Karla:ital,wght@0,200..800;1,200..800&display=swap' },
      ],
    }
  },
  setup() {
    const showModal = ref(false)
    const modalCaption = ref('')

    const openModal = () => {
      showModal.value = true
      modalCaption.value = 'Resume (Tanner Green - 2024)'
    }

    const closeModal = () => {
      showModal.value = false
    }

    return {
      showModal,
      modalCaption,
      openModal,
      closeModal
    }
  }
}
</script>


<style lang="css">

@import url('https://fonts.googleapis.com/css2?family=Karla:wght@400;600&family=Playfair+Display:wght@600&display=swap');

body {
  font-family: 'Karla', sans-serif;
  margin: 0;
  padding: 0;
}

h2 {
  font-family: 'Playfair Display', serif;
  font-size: 2rem;
  font-weight: 600;
}

.bg {
    background-image: url("/assets/background.png");
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
    min-height: 100vh;
    width: 100vw;
    overflow-x: hidden;
    padding-bottom: 100px;
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

.containerdiv {
  width: 100%;
}

.containerdiv {
  background: #fff;
  border-radius: 16px;
  padding: 2rem;
  box-shadow: 0 20px 40px rgba(0,0,0,0.1);
  width: 80%;
  max-width: 960px;
  margin-top: 125px;
  margin-left: auto;
  margin-right: auto;
}

.hero-heading {
  background: #c4e2bc;
  padding: 1.5rem;
  border-radius: 16px 16px 0 0;
  text-align: center;
  font-size: 1.75rem;
}

.intro-section {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  margin-top: 2rem;
  align-items: center;
  justify-content: center;
}

.avatar {
  border-radius: 16px;
  max-width: 150px;
  box-shadow: 0 10px 20px rgba(0,0,0,0.1);
}

.intro-text {
  max-width: 600px;
  text-align: left;
}


.intro-text p {
  font-size: 1.2rem;
  line-height: 1.6;
}

.pagebtns {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}

.btn-main {
  background-color: #688665;
  color: white;
  border: none;
  border-radius: 50px;
  padding: 0.6rem 1.5rem;
  font-weight: 600;
  font-size: 1rem;
  transition: all 0.3s ease;
  cursor: pointer;
}

.btn-main:hover {
  background-color: #4d654d;
  transform: translateY(-2px);
}

.webp-wrapper {
  display: flex;
  justify-content: center;
  gap: 0.5rem;
}

.webp-animation {
  width: 275px; 
  transform: scaleX(1); 
  height: 50px;
}

.webp-animation.flipped {
  transform: scaleX(-1); 
}

@media screen and (max-width: 768px) {
  .intro-section {
    flex-direction: column;
    text-align: center;
  }

  .avatar {
    margin-bottom: 1rem;
  }

  .pagebtns {
    justify-content: center;
    width: 100%;
  }

  .btncontainer {
    width: 100%;
  }

  .btn-main {
    width: 100%;
  }

  .webp-animation {
  width: 150px; 
  margin-top: 1rem;
  transform: scaleX(1);
  height: auto;
}

.containerdiv {
  background: #fff;
  border-radius: 16px;
  padding: 1rem;
  box-shadow: 0 20px 40px rgba(0,0,0,0.1);
  width: 90%;
  max-width: 960px;
  margin-top: 100px;
}

.supimg {
  display: none;
}

}

.modal {
  display: none; /* Hidden by default */
  position: fixed; /* Stay in place */
  z-index: 1001; /* Sit on top */
  padding-top: 100px; /* Location of the box */
  left: 0;
  top: 0;
  width: 100%; /* Full width */
  height: 100%; /* Full height */
  overflow: auto; /* Enable scroll if needed */
  background-color: rgb(0,0,0); /* Fallback color */
  background-color: rgba(0,0,0,0.9); /* Black w/ opacity */
}

.modal.show {
  display: block;
}

.close {
  position: fixed; /* Instead of absolute */
  top: 20px;
  right: 30px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  z-index: 1002; /* One level above modal */
  background: transparent;
  border: none;
  cursor: pointer;
  transition: 0.3s;
}

.featurebtn {
  background-color: #688665;
  color: white;
  border: none;
  border-radius: 50px;
  padding: 0.6rem 1.5rem;
  font-weight: 600;
  font-size: 1rem;
  transition: all 0.3s ease;
  cursor: pointer;
  width: 100%;
}

.featurebtn:hover {
  background-color: #4d654d;
  transform: translateY(-2px);
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}

.featured-section {
  margin-left: auto;
  margin-right: auto;
}

</style>
