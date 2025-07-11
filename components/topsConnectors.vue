<template>
    <div class="modaldiv">
      <h2 class="mb-4">Project Lead: Design & Development for topsconnectors.com</h2>
      <p class="mb-4">TopsConnectors.com was created at the request of Titan Building Products CEO Richard Bergman to serve as a dedicated showcase for the company’s new pergola hardware line—TOPS Connectors. I was tasked with designing and developing a branded sister site that would highlight the system’s modular features while directing traffic back to our e-commerce platform at <strong>store.decksgo.com</strong>. The goal was to establish a clean, product-focused experience that could grow alongside the expanding product line.</p>
      <a class="btn-main" href="https://topsconnectors.com/" target="blank">Visit topsconnectors.com</a>
      <div class="mt-5 mb-5">
        <h2>Design Phase</h2>
      </div>
      <img src="/assets/topsconnectors wireframes.png" alt="wireframes">
    
      
      <div class="row align-items-start d-flex align-items-center mt-5 mb-5">
        <div class="col-12 col-md-4">
          <div>
            <img src="/assets/topsconnectors wireframes2.png" alt="wireframes2">
          </div>
        </div>
        <div class="col-12 col-md-8">
          <p>
            The initial design phase for <strong>TOPS Connectors</strong> began with <strong>wireframing</strong> and <strong>prototyping</strong> in Figma, where we laid the groundwork for a <strong>streamlined</strong> and <strong>intuitive user experience</strong>. While some elements evolved throughout development—such as <strong>layout refinements</strong> and a color change from 
            <span style="color: #794a4a;"><strong>#794a4a</strong></span> to 
            <span style="color: #a8690a;"><strong>#a8690a</strong></span> to better align with our parent brand’s identity—the core <strong>UX principles</strong> remained consistent. 
            The original design philosophy centered around a <strong>category-based navigation system</strong>, with sections like <strong>Shade</strong>, <strong>Privacy</strong>, and <strong>TOPS Connectors</strong>. 
            Within each category, a <strong>sub-navigation</strong> would allow users to browse individual products <strong>seamlessly</strong> without jumping to separate pages. 
            This approach enabled <strong>dynamic updates</strong> across the page, including product images, descriptions, components, and store links, ensuring a <strong>smooth</strong> and <strong>cohesive</strong> browsing experience.
          </p>


        </div>
      </div>

      <div class="row align-items-start d-flex align-items-center mt-5 mb-5">
        <div class="col-12 col-md-6">
          <div>
            <h2>Development Phase</h2>
            <p>
              One of the first things we developed for <strong>TOPS Connectors</strong> was a <strong>custom JavaScript application</strong> designed to play seamless <strong>WebP animations</strong> created by our in-house 3D artist. When users clicked on a specific connector, the application would dynamically display an animation that <strong>added or removed modular components</strong> depending on the selected product. This visually reinforced the core <strong>selling point</strong> of the system—<strong>modularity</strong>. As users cycled through connectors like the TRI-TOP™, QUATRA-TOP™, and PENTA-TOP™, transition animations made the evolution between each product type clear and <strong>interactive</strong>, helping customers understand how the system could <strong>grow or adapt</strong> to their needs in real time.
            </p>

            
          </div>
        </div>
        <div class="col-12 col-md-6">
         <img src="/assets/tops animation app.webp" alt="tops webp javascript animation">

        </div>
      </div>

      <div class="row align-items-start d-flex align-items-center mt-5 mb-5">
        <div class="col-12 col-md-6">
          <div>
            <img src="/assets/tops animation for shade.webp" alt="tops webp javascript animation final version">  
          </div>
        </div>
        <div class="col-12 col-md-6">
          <p>
            The same <strong>logic</strong> used for the TOPS animation system was later adapted across each <strong>category page</strong>—including <strong>Shade</strong>, <strong>Privacy</strong>, and <strong>Connectors</strong>—to create a consistent and interactive product browsing experience. Instead of loading separate product pages, users could seamlessly <strong>cycle through product variants</strong> within a single page. As they did, the application would dynamically update the <strong>product description</strong>, <strong>component list</strong>, <strong>imagery</strong>, and <strong>buy links</strong> in real time. This approach kept the experience fast and fluid while reinforcing the idea that all TOPS products are part of a <strong>modular and unified system</strong>.
          </p>
        </div>
      </div>
      <div class="mt-5 mb-5">
        <p class="mb-4">
          The website was ultimately built using <strong>WordPress</strong> with <strong>Beaver Builder</strong> for layout control, alongside <strong>custom JavaScript</strong>, <strong>HTML</strong>, and <strong>CSS</strong> for interactive and visual features. I also implemented some targeted <strong>PHP</strong> on the Pergola Kits page to enable <strong>filtering functionality</strong>, helping users quickly find the right configuration. This blend of tools allowed us to deliver a fast, modular, and brand-consistent digital experience that showcases the full potential of the TOPS Connector system.
        </p>
        <a class="btn-main" href="https://topsconnectors.com/" target="blank">Visit topsconnectors.com</a>
      </div>
    </div>
  </template>

<script setup>

</script>

<style lang="css">

    .nav-link {
        color: white;
    }
    
    .nav-link:hover {
        color: white;
    }

    .modaldiv {
        margin-left: 10%;
        margin-right: 10%;
        color: white;
        font-size: 1.2rem;
        line-height: 1.6;
    }

    img {
        width: 100%;
        border-radius: 20px;
    }

   

    .video-wrapper {
      position: relative;
      width: 100%;
      padding-bottom: 56.25%; /* 16:9 ratio */
      height: 0;
      overflow: hidden;
      border-radius: 20px;
    }

    .video-wrapper iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: none;
    }


    @media screen and (max-width: 768px) {
        iframe {
          width: 100%;
          border-radius: 0px;
        }

        p {
          padding-top: 20px;
          padding-bottom: 20px;
        }
    
    }
</style>