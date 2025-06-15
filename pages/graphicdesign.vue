<template>
    <div class="bg">
       <div class="container pt-12" data-aos="fade-up" data-aos-duration="1000">
         <div class="title">
             <h2 class="text-center hero-heading">
                Personal & Professional Graphic Design Work
             </h2>
         </div>
   
         <div class="row grid g-4" data-masonry='{"percentPosition": true }'>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/soil test kit second headline mobile.png" class="card-img-top" alt="soil test kit email banner" />
      <div class="card-body">
        <p class="card-text">Soil Test Kit Email Banner</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/topstri-top4x4.png" class="card-img-top" alt="TOPS TRI-TOP box sticker" />
      <div class="card-body">
        <p class="card-text">TOPS Connectors: TRI-TOP Box Sticker</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/killbill.png" class="card-img-top" alt="Kill Bill Vector Art" />
      <div class="card-body">
        <p class="card-text">Kill Bill Vector Art</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/keapbannerBF-1.png" class="card-img-top" alt="Black Friday Email Banner" />
      <div class="card-body">
        <p class="card-text">Black Friday Email Banner</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/topsshadesail10x10.png" class="card-img-top" alt="TOPS Shade Sail box sticker" />
      <div class="card-body">
        <p class="card-text">TOPS Connectors: Shade Sail Box Sticker</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/pergolaBracketInstall.png" class="card-img-top" alt="TOPS pergola bracket install line art" />
      <div class="card-body">
        <p class="card-text">TOPS Pergola Bracket Line Art (Installation Manual)</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/louvertops2.png" class="card-img-top" alt="louver tops connecting to hubs" />
      <div class="card-body">
        <p class="card-text">Louver Tops Line Art (Installation Manual)</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/LouverTops Box Sticker.png" class="card-img-top" alt="Louver Tops Box Sticker" />
      <div class="card-body">
        <p class="card-text">Louver Tops Box Sticker</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/topsAddOnInstall.png" class="card-img-top" alt="TOPS pergola connectors install line art" />
      <div class="card-body">
        <p class="card-text">TOPS Pergola Connectors Line Art (Installation Manual)</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/St. Patricks Day (last chance).png" class="card-img-top" alt="St. Patricks Day Email Banner" />
      <div class="card-body">
        <p class="card-text">St. Patricks Day Email Banner</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/topspostbase.png" class="card-img-top" alt="TOPS Post Base box sticker" />
      <div class="card-body">
        <p class="card-text">TOPS Connectors: Post Base Box Sticker</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/squidart.png" class="card-img-top" alt="squid art" />
      <div class="card-body">
        <p class="card-text">Squid "Flash" Art</p>
      </div>
    </div>
  </div>
  <div class="col-12 col-md-6 col-lg-4 grid-item" data-aos="fade-up" data-aos-duration="1000">
    <div class="card">
      <img src="/assets/graphicdesign/louvertops1.png" class="card-img-top" alt="louver tops connecting to shade board" />
      <div class="card-body">
        <p class="card-text">Louver Tops Line Art (Installation Manual)</p>
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
    import { onMounted, ref } from 'vue'
    import { useHead } from '#imports'

    const showModal = ref(false)
    const selectedComponent = ref(null)

    function closeModal() {
    showModal.value = false
    selectedComponent.value = null
    }

    useHead({
    script: [
        {
        src: 'https://cdn.jsdelivr.net/npm/masonry-layout@4.2.2/dist/masonry.pkgd.min.js',
        integrity: 'sha384-GNFwBvfVxBkLMJpYMOABq3c+d3KnQxudP/mGPkzpZSTYykLBNsZEnG2D9G/X/+7D',
        crossorigin: 'anonymous',
        async: true
        },
        {
        src: 'https://unpkg.com/imagesloaded@5/imagesloaded.pkgd.min.js',
        async: true
        }
    ]
    })

    onMounted(() => {
    const interval = setInterval(() => {
        if (window.Masonry && window.imagesLoaded) {
        clearInterval(interval)
        const grid = document.querySelector('.grid')

        window.imagesLoaded(grid, () => {
            new window.Masonry(grid, {
            itemSelector: '.grid-item',
            percentPosition: true,
            })
        })
        }
    }, 100)
    })

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
   