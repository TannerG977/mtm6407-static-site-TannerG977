<template>
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
            <NuxtLink class="nav-link fw-medium" to="/Contact">Contact</NuxtLink>
        </li>
      </ul>
    </div>
  </div>
</nav>
    </div>
</template>

<script setup>
    
</script>

<style lang="css" scoped>
 .nav-link {
  color: #688665 !important ;
 }

 .nav-link:hover {
  color: #9fd4aa !important ;
  font-size: 110%;
  text-decoration: underline;
 }

</style>