<script setup>
   import './assets/base.css' //Importando configuração Básica 
   import './assets/mobile.css' 
   import './assets/tablet.css' 
   import './assets/desktop.css' 
   import 'bootstrap/dist/css/bootstrap.min.css' //Importando CSS Bootstrap
   import 'bootstrap/dist/js/bootstrap.bundle.min.js' //Importando JS Bootstrap
</script>

<template>
  <nav id="Nav" class="navbar navbar-expand-sm py-2">
    <div class="container-fluid">
      <button class="navbar-toggler fs-1 ms-1" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon p-4"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-lg-end" id="navbarNav">
        <ul class="navbar-nav justify-content-around me-lg-4">
          <li class="nav-item">
            <a class="nav-link" href="#">Inicio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Projetos</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Sobre Mim</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contato</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <main>
     
  </main>
</template>

<style scoped>
  #Nav{
    background-color: var(--Nav-Background);
    box-shadow: 0 1px 6px 4px var(--Box-Shadow-Color);
  }
  .nav-link{
    font-family: "Roboto", sans-serif;
    text-transform: uppercase;
    font-size: var(--Nav-Font);
    color:var(--Color-Secondary);
    &:hover{
      color: var(--Color-Primary);
      transition: 0.3s ease; 
    }
  }
</style>
