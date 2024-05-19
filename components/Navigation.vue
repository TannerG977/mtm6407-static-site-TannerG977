<template>
  <head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Karla:ital,wght@0,200..800;1,200..800&display=swap" rel="stylesheet">
  </head>
  <main class="shadow-lg">
    <div>
        <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <NuxtLink class="navbar-brand" to="/">
      <img src="/assets/nav-logo.png" alt="Logo" width="50" height="50" class="d-inline-block align-text-top">
    </NuxtLink>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <NuxtLink class="nav-link button-18 me-2" aria-current="page" to="/">Home</NuxtLink>
        </li>
        <li class="nav-item">
            <NuxtLink class="nav-link button-18 me-2" to="/Resume">Resume</NuxtLink>
        </li>
        <li class="nav-item">
            <NuxtLink class="nav-link button-18 me-2" to="/design">Design/Video</NuxtLink>
        </li>
        <li class="nav-item">
            <NuxtLink class="nav-link button-18 me-2" to="/coding">Web Dev</NuxtLink>
        </li>
        <li class="nav-item">
            <NuxtLink class="nav-link button-18 me-2" to="/Contact">Contact</NuxtLink>
        </li>
      </ul>
      <h4 class="text-center">Tanner Green</h4>
    </div>
  </div>
  
</nav>
    </div>
    <div class="banner text-center">
    </div>
  </main>
</template>

<script setup>
    
</script>

<style lang="css" scoped>

h4 {
  color: #688665;
  padding-right: 15px;
}

main {
  overflow: hidden;
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 1000;
  font-family: "Karla", sans-serif;
}

 .banner {
    background-color: #9fd4aa;
    height: 10px;
}

.button-18 {
  align-items: center;
  background-color: #c4e2bc !important;
  border: 0;
  border-radius: 100px;
  box-sizing: border-box;
  color: black;
  cursor: pointer;
  display: inline-flex;
  font-size: 16px;
  font-weight: 600;
  justify-content: center;
  line-height: 20px;
  max-width: 480px;
  min-height: 40px;
  min-width: 0px;
  overflow: hidden;
  width: 125px;
  text-align: center;
  touch-action: manipulation;
  transition: background-color 0.167s cubic-bezier(0.4, 0, 0.2, 1) 0s, box-shadow 0.167s cubic-bezier(0.4, 0, 0.2, 1) 0s, color 0.167s cubic-bezier(0.4, 0, 0.2, 1) 0s;
  user-select: none;
  -webkit-user-select: none;
  vertical-align: middle;
  font-size: 15px;
}

.button-18:hover { 
  background-color: #688665 !important;
  color: #ffffff;
}

@media only screen and (max-width: 1000px){
  
  h4 {
    display: none;
  }

  li {
    text-align: center;
    margin-bottom: 12px;
  }

  .button-18 {
    width: 200px !important;
  }
}

</style>