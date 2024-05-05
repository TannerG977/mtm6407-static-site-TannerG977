<template>
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
          <NuxtLink class="nav-link fw-medium" aria-current="page" to="/">Home</NuxtLink>
        </li>
        <li class="nav-item">
            <NuxtLink class="nav-link fw-medium" to="/Resume">Resume</NuxtLink>
        </li>
        <li class="nav-item">
            <NuxtLink class="nav-link fw-medium" to="/design">Design/Video</NuxtLink>
        </li>
        <li class="nav-item">
            <NuxtLink class="nav-link fw-medium" to="/coding">Coding</NuxtLink>
        </li>
        <li class="nav-item">
            <NuxtLink class="nav-link fw-medium" to="/Contact">Contact</NuxtLink>
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
}

 .nav-link {
  color: #688665 !important ;
 }

 .nav-link:hover {
  color: #9fd4aa !important ;
  font-size: 110%;
  text-decoration: underline;
 }

 .banner {
    background-color: #9fd4aa;
    height: 20px;
}

@media only screen and (max-width: 700px){
  
  h4 {
    display: none;
  }
}

</style>