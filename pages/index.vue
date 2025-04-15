<template>
  <div class="main-bg">
    <div class="containerdiv">
      <h2 class="hero-heading">Welcome to my web portfolio.</h2>
      <div class="intro-section">
        <img class="avatar" alt="avatar" src="/assets/profilepic.png" height="150" />
        <div class="intro-text">
          <p>
            My name is Tanner Green, and I am a web developer, videographer, and graphic designer. This site showcases projects that reflect the skills I’ve developed throughout my professional and academic career. Feel free to explore using the buttons below.
          </p>
        </div>
        <div class="pagebtns">
            <NuxtLink to="/Resume" class="btncontainer"><button class="btn-main">Resume</button></NuxtLink>
            <NuxtLink to="/design" class="btncontainer"><button class="btn-main">Design/Video</button></NuxtLink>
            <NuxtLink to="/coding" class="btncontainer"><button class="btn-main">Web Dev</button></NuxtLink>
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
        <div class="project-card" data-aos="zoom-in" data-aos-once="true">
          <img src="#" alt="Project 1" />
          <h4>Project Title One</h4>
          <p>A brief description of the project, tech used, or design style.</p>
        </div>
        <div class="project-card" data-aos="zoom-in" data-aos-delay="100" data-aos-once="true">
          <img src="#" alt="Project 2" />
          <h4>Project Title Two</h4>
          <p>This one was built with JavaScript and custom CSS animations.</p>
        </div>
        <div class="project-card" data-aos="zoom-in" data-aos-delay="100" data-aos-once="true">
          <img src="#" alt="Project 3" />
          <h4>Project Title Three</h4>
          <p>A web development piece using Nuxt and API integrations.</p>
        </div>
      </div>
    </div>
  </div>
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

.main-bg {
  background: url('/assets/background.png') center/cover fixed no-repeat;
  min-height: 100vh;
  display: flex;
  align-items: center;
  padding: 2rem 0;
}

.main-bg {
  display: flex;
  flex-direction: column;
  gap: 3rem; /* adds vertical space between intro and projects */
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
  margin-top: 100px;
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
}

</style>
