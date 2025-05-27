<template>
    <div class="modaldiv">
      <h2 class="mb-4">Free deck plans distribution & email lead collection site.</h2>
      <p class="mb-4">Plans.DecksGo.com is a lead-generation microsite offering free downloadable deck plans in exchange for email signups. I led a full <strong>redesign</strong> of the site, modernizing its layout and user experience while creating many of the visual assets myself—including <strong>banners</strong>, <strong>advert cards</strong>, and promotional graphics.<br><br> On the development side, I integrated a <strong>custom app</strong> using the <strong>Attentive CRM API</strong>, enabling seamless transfer of contact data from Gravity Forms with <strong>AI-assisted PHP scripting</strong>. To maximize reach, I also executed a comprehensive <strong>SEO</strong> and <strong>performance optimization</strong> strategy, which has propelled the site to the <strong>#2 ranking</strong> for the competitive search term <strong>“free deck plan PDF”</strong>, outranking major players like Home Depot.</p>
      <a class="btn-main" href="https://plans.decksgo.com" target="blank">Visit plans.decksgo.com</a>


        <div class="row align-items-start d-flex align-items-center mt-5 mb-5">
            <div class="col-12 col-md-6">
          <div>
            <h2 class="mt-4 mt-md-0">Re-Design</h2>
            <p>
             As part of the redesign, I focused on improving the overall user experience by implementing a cleaner, more intuitive interface. One of the key enhancements was the addition of a <strong>secondary navigation system</strong> that allows users to easily filter deck plans by type—such as ground level, elevated, or multi-tier. <br><br>This improvement significantly reduced friction in the user journey and helped users quickly find the plans most relevant to their needs. I also overhauled the site’s visual style to better align with our brand, introducing a more modern, consistent look across typography, spacing, and component design.
            </p>
          </div>
        </div>
            <div class="col-12 col-md-6">
            <ul class="nav nav-tabs" id="myTab" role="tablist">
            <li class="nav-item" role="presentation">
                <button class="nav-link active" id="home-tab" data-bs-toggle="tab" data-bs-target="#new" type="button" role="tab" aria-controls="home" aria-selected="true">New Home Page</button>
            </li>
            <li class="nav-item" role="presentation">
                <button class="nav-link" id="profile-tab" data-bs-toggle="tab" data-bs-target="#old" type="button" role="tab" aria-controls="profile" aria-selected="false">Old Home Page</button>
            </li>
            </ul>
            <div class="tab-content" id="myTabContent">
            <div class="tab-pane fade show active mt-4" id="new" role="tabpanel" aria-labelledby="home-tab"><img src="assets\plans site screengrabs\new homepage.png" alt="new plans.decksgo.com homepage"></div>
            <div class="tab-pane fade mt-4" id="old" role="tabpanel" aria-labelledby="profile-tab"><img src="assets\plans site screengrabs\old homepage.png" alt="old plans.decksgo.com homepage"></div>
        </div>

        </div>
      </div>
      
      <div class="row align-items-start d-flex align-items-center mt-5 mb-5">
        <div class="col-12 col-md-6">
          <div>
            <img src="\assets\plans site screengrabs\plans.decksgo wireframes.png" alt="wireframes">
          </div>
        </div>
        <div class="col-12 col-md-6">
          <p>To create the updated design, I used <strong>Adobe Illustrator</strong> and <strong>Photoshop</strong> to develop custom visual assets, including plan thumbnails, banners, and promotional graphics. I then mapped out the new layout and user flows in <strong>Figma</strong>, building wireframes that guided the redesign. Once the design was finalized, I implemented all changes using <strong>HTML</strong> and <strong>CSS</strong> directly within the theme’s page templates, ensuring a seamless transition from concept to live site. These enhancements not only modernized the aesthetic but also contributed to faster page performance and increased user engagement.</p>

        </div>
      </div>

      <div class="row align-items-start d-flex align-items-center mt-5 mb-5">
        <div class="col-12 col-md-6">
          <div>
            <h2>Development</h2>
             <p>On the development side, one of the first issues I addressed was the lack of product visibility on the site. Despite high traffic, the page wasn’t promoting any of our storefront items. To solve this, I designed a set of promotional <strong>product cards</strong> and strategically placed them between existing <strong>deck plan cards</strong>. I used styled div elements interspersed throughout the layout, then wrote a <strong>JavaScript array</strong> to dynamically assign each card a <strong>background image</strong> and <strong>button link</strong> to relevant products. <br><br> To keep the experience fresh and prevent ad fatigue, I implemented <strong>randomized positioning</strong> for the cards on each page load. This lightweight solution allowed us to monetize traffic without compromising the user experience.</p>
            
          </div>
        </div>
        <div class="col-12 col-md-6">
         <img src="\assets\plans site screengrabs\product cards.png">

        </div>
      </div>

      <div class="row align-items-start d-flex align-items-center mt-5 mb-5">
       
       
           <p>The second major development task involved migrating our email sign-up process from Keap to <strong>Attentive CRM</strong>. Since there is no native Gravity Forms integration with Attentive, I built a custom connection using their <strong>Subscribers API</strong>. This required mapping form fields to Attentive’s contact schema, developing a <strong>custom app within the CRM</strong>, and writing <strong>PHP functions</strong> to handle the data transfer securely.<br><br>I used <strong>AI-assisted coding</strong> to generate and validate the PHP logic inserted into the site’s <strong>functions.php</strong> file. Now, whenever a user submits a form to download a deck plan, their information is automatically passed to Attentive, creating new subscribers in real-time—streamlining our lead capture and follow-up efforts.</p>
      </div>

      <div class="row align-items-start d-flex align-items-center mt-5 mb-5">
        <div class="col-12 col-md-8">
          <div>
            <h2>SEO Optimization</h2>
            <p>
              To maximize visibility and organic traffic, I conducted a targeted <strong>SEO optimization</strong> campaign focused on the high-intent keyword phrase <strong>“free deck plans PDF.”</strong> This included refining on-page elements such as <strong>meta titles</strong>, <strong>descriptions</strong>, and <strong>header tags</strong> to align with search intent, as well as optimizing <strong>image alt text</strong> and improving overall <strong>page load speed.</strong><br><br> 
              I also implemented structured content and internal linking strategies to enhance crawlability and user engagement. As a result of these efforts, Plans.DecksGo.com now ranks consistently within the <strong>top 3 search results</strong> for this term—outperforming industry giants like Home Depot—and driving steady, qualified traffic to our email capture funnel.
            </p>
          </div>
        </div>
        <div class="col-12 col-md-4">
          <img src="/assets/plans site screengrabs/performance.png" class="img-fluid" alt="Performance Metrics">
        </div>
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