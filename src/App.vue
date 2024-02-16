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

  <main id="Main" class="container-fluid">
    <div class="row mt-4">
      <div class="col-lg-5 col-12 d-flex justify-content-center">
        <img class="Minha-Foto rounded-circle" src="./assets/midia/minha-foto.jpg" alt="">
      </div>
      <div class="Frase-e-icones col-lg-6 col mt-sm-5">
        <h2 class="Frase-e-icones--txt1">Olá sou Matheus,</h2>
        <h2 class="Frase-e-icones--txt2">Desenvolvedor Web</h2>
        <ul class="row gap-lg-3 mt-sm-4 row-gap-4 mt-2 mt-sm-5 justify-content-center">
          <li class="col-lg-2 col-sm-3 col-4 justify-content-center d-flex"> <img src="./assets/midia/icons/html-5-svgrepo-com.svg" alt=""> </li>
          <li class="col-lg-2 col-sm-3 col-4 justify-content-center d-flex"> <img src="./assets/midia/icons/css-3-svgrepo-com.svg" alt=""> </li>
          <li class="col-lg-2 col-sm-3 col-4 justify-content-center d-flex"> <img src="./assets/midia/icons/js-svgrepo-com.svg" alt=""> </li>
          <li class="col-lg-2 col-sm-3 col-4 justify-content-center d-flex"> <img src="./assets/midia/icons/node-js-svgrepo-com.svg" alt=""> </li>
          <li class="col-lg-2 col-sm-3 col-4 justify-content-center d-flex"> <img src="./assets/midia/icons/bootstrap-4-logo-svgrepo-com.svg" alt=""> </li>
          <li class="col-lg-2 col-sm-3 col-4 justify-content-center d-flex"> <img src="./assets/midia/icons/vue-svgrepo-com.svg" alt=""> </li>
          <li class="col-lg-2 col-sm-3 col-4 justify-content-center d-flex"> <img src="./assets/midia/icons/sass-svgrepo-com.svg" alt=""> </li>
          <li class="col-lg-2 col-sm-3 col-4 justify-content-center d-flex"> <img src="./assets/midia/icons/jquery-svgrepo-com.svg" alt=""> </li>
          <li class="col-lg-2 col-sm-3 col-4 justify-content-center d-flex"> <img src="./assets/midia/icons/python-svgrepo-com.svg" alt=""> </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<style scoped>
  /* Configurações globais e para Desktops ou TVs*/
  #Nav{
    background-color: var(--Nav-Background);
    box-shadow: 0 1px 6px 4px var(--Box-Shadow-Color);
  }
  #Nav .nav-link{
    font-family: "Roboto", sans-serif;
    text-transform: uppercase;
    font-size: var(--Nav-Font);
    color:var(--Color-Secondary);
    &:hover{
      color: var(--Color-Primary);
      transition: 0.3s ease; 
    }
  }

  .Frase-e-icones ul li img{
      animation: rotateHorizontal 5s infinite linear;
  }
  .Frase-e-icones ul{
      list-style: none;
      padding-right: 32px;
      width: 100%; 
      margin: 0 auto;
  }
  @keyframes rotateHorizontal {
    0% {
      transform: rotateY(0deg);
    }
    100% {
      transform: rotateY(360deg);
    }
  } 
</style>
