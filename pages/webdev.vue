<template>
    <div class="bg">
       <div class="container pt-12" data-aos="fade-up" data-aos-duration="1000">
         <div class="title">
             <h2 class="text-center hero-heading">
               Web Design & Development Projects
             </h2>
         </div>
   
         <div class="row g-4">
            <div
                class="col-12 col-md-6 col-lg-4"
                v-for="(webdev, index) in webdevs"
                :key="index"
                data-aos="fade-up"
                :data-aos-delay="index * 100"  
                >
                <div class="rounded-4 shadow-lg bg-white overflow-hidden h-100 d-flex flex-column">
                    <div class="vidcontainer">
                    <img :src="webdev.src" alt="thumbnail image" class="rounded-4">
                    </div>
                    <div class="p-4 d-flex flex-column justify-content-between h-100">
                    <h5 class="fw-bold mb-3">{{ webdev.title }}</h5>
                    <p v-html="webdev.description" class="mb-0 text-sm"></p>
                    <button v-bind:id="webdev.id"  @click="openModal(webdev.component)">More Details</button>
                    </div>
                </div>
                </div>

         </div>
   
         
       </div>
     </div>
     <div class="modal" :class="{ 'show': showModal }">
        <span class="close" @click="closeModal">&times;</span>
        <component :is="selectedComponent" />
    </div>
   </template>
   
   <script setup>
    import FreeDeckPlans from '~/components/freeDeckPlans.vue';
import DFAFBAD from '/components/DFA-FB-AD.vue'
    import balusterCalculator from '/components/balusterCalculator.vue'

   const webdevs = [
    {
       title: "Deck Plans Distribution Site (Redesign, development & SEO Optimization)",
       src: "/assets/plans.decksgo.com.png",
       description: `This is a simple contact book, web application I created. The website was created using Vue 3, Vite, Vue Router and Bootstrap. The site allows the user to create contacts and edit existing ones. In addition, you can search contacts, filter alphabetically by last name or first name and delete existing contacts. All contact data is saved to a user's local storage so when the page is reloaded, contacts remain on the page.`,
       component: FreeDeckPlans,
     },
    {
       title: "Baluster Quantity Calculator",
       src: "/assets/baluster calculator.png",
       description: `This is a simple contact book, web application I created. The website was created using Vue 3, Vite, Vue Router and Bootstrap. The site allows the user to create contacts and edit existing ones. In addition, you can search contacts, filter alphabetically by last name or first name and delete existing contacts. All contact data is saved to a user's local storage so when the page is reloaded, contacts remain on the page.`,
       component: balusterCalculator,
     },
     {
       title: "Contact Book",
       src: "/assets/contactbook.png",
       description: `This is a simple contact book, web application I created. The website was created using Vue 3, Vite, Vue Router and Bootstrap. The site allows the user to create contacts and edit existing ones. In addition, you can search contacts, filter alphabetically by last name or first name and delete existing contacts. All contact data is saved to a user's local storage so when the page is reloaded, contacts remain on the page.`,
       component: DFAFBAD,
     },
   ];

    const showModal = ref(false)
    const selectedComponent = ref(null)

    const openModal = (component) => {
    selectedComponent.value = component
    showModal.value = true
    }

    const closeModal = () => {
    showModal.value = false
    selectedComponent.value = null
    }
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
     width: 100%;
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
  background-color: #000;
  overflow: hidden; /* Ensures the image doesn't overflow */
}

.vidcontainer img {
  width: 100%;  /* Make the image span the full width of its container */
  height: auto;  /* Maintain aspect ratio */
  display: block; /* Remove any inline spacing issues */
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

 button {
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

button:hover {
  background-color: #4d654d;
  transform: translateY(-2px);
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
   