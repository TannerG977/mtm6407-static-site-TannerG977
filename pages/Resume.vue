<template>
    <body class="bg">
        <div>
        <div class="text-center mt-5 grid">
            <img class="shadow-lg transition rounded-4 mt-4" src="/assets/Resume.png" alt="Resume" style="width:100%;max-width:250px" @click="openModal">
            <img class="img-2 shadow-lg transition rounded-4 mt-4" src="/assets/CV.png" alt="CV" style="width:100%;max-width:250px" @click="openModal2">
        </div>
        <!-- Modal -->
        <div class="modal" :class="{ 'show': showModal }">
            <!-- The Close Button -->
            <span class="close" @click="closeModal">&times;</span>
            <!-- Modal Content (The Image) -->
            <img class="modal-content" src="/assets/Resume.png" alt="Resume" id="img01">
            <!-- Modal Caption (Image Text) -->
            <div id="caption">{{ modalCaption }}</div>
        </div>
        <div class="modal2" :class="{ 'show': showModal2 }">
            <!-- The Close Button -->
            <span class="close" @click="closeModal2">&times;</span>
            <!-- Modal Content (The Image) -->
            <img class="modal-content2" src="/assets/CV.png" alt="CV" id="img02">
            <!-- Modal Caption (Image Text) -->
            <div id="caption2">{{ modalCaption2 }}</div>
        </div>
        </div>
    </body>
  </template>
  
  <script setup>
  import { ref } from 'vue';

  //modal1
  
  const showModal = ref(false);
  const modalCaption = ref('');
  
  function openModal() {
    showModal.value = true;
    modalCaption.value = 'Resume (Tanner Green - 2024)';
  }
  
  function closeModal() {
    showModal.value = false;
  }

  //modal 2
  const showModal2 = ref(false);
  const modalCaption2 = ref('');
  
  function openModal2() {
    showModal2.value = true;
    modalCaption2.value = 'CV (Tanner Green - 2024)';
  }
  
  function closeModal2() {
    showModal2.value = false;
  }
  </script>
  
  <style lang="css" scoped>

  body {
      padding-top: 50px;
  }

    @media only screen and (min-width: 701px){

        .img-2 {
            margin-left: 40px;
        }

    }

    .bg {
        background-image: url("/assets/background.png") !important;
        background-size: cover;
        background-attachment: fixed;
        background-position: center;
        height: 100vh;
        width: 100vw;
    }

  .transition {
    transition: all .2s ease-in-out;
  }
  
  .transition:hover {
    transform: scale(1.1);
    cursor: pointer;
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

.modal2 {
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


/* Modal Content (Image) */
.modal-content {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
}

.modal-content2 {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
  border-radius: 10px;
}

/* Caption of Modal Image (Image Text) - Same Width as the Image */
#caption {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
  text-align: center;
  color: #ccc;
  padding: 10px 0;
  height: 150px;
}

#caption2 {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
  text-align: center;
  color: #ccc;
  padding: 10px 0;
  height: 150px;
}

/* Add Animation - Zoom in the Modal */
.modal-content, #caption {
  animation-name: zoom;
  animation-duration: 0.6s;
}

.modal-content2, #caption2 {
  animation-name: zoom;
  animation-duration: 0.6s;
}

@keyframes zoom {
  from {transform:scale(0)}
  to {transform:scale(1)}
}

/* The Close Button */
.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  transition: 0.3s;
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}


/* 100% Image Width on Smaller Screens */
@media only screen and (max-width: 700px){
  .modal-content {
    width: 100%;
  }

  .modal-content2 {
    width: 100%;
  }

  .grid {
    display: grid;
    justify-content: center;
  }

  img {
    margin-top: 25px;
  }

  .img-2 {
    margin-bottom: 100px;
  }



}
  
  /* Show the modal when showModal is true */
  .modal {
    display: none;
    /* Your other modal styles */
  }

  .modal2 {
    display: none;
    /* Your other modal styles */
  }
  
  .modal.show {
    display: block;
  }

  .modal2.show {
    display: block;
  }
  </style>
  