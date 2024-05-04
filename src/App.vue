<script setup>
import { ref } from 'vue';

const num = ref(0);
</script>

<template>
<<<<<<< HEAD
  <link rel="stylesheet" href="../src/assets/home.css">
  <nav class="navbar navbar-expand-lg">
=======
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark">
>>>>>>> be1db158649fe924aa67d78d2b69b2ab15671d30
    <div class="container-fluid">
      <RouterLink class="navbar-brand" to="/">Rick and Morty</RouterLink>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <RouterLink class="nav-link active" aria-current="page" to="/">Início</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link" to="/about">Sobre</RouterLink>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <div class="main">
    <router-view></router-view>
  </div>

<<<<<<< HEAD
  <footer>
=======
  <footer class="bg-dark text-light">
>>>>>>> be1db158649fe924aa67d78d2b69b2ab15671d30
    <div>Unimar | ADS | {{ new Date().getFullYear()}}</div>
  </footer>
</template>

<style>
<<<<<<< HEAD

=======
 footer{
    position: fixed;
    bottom: 0;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 55px;  
  }
>>>>>>> be1db158649fe924aa67d78d2b69b2ab15671d30
</style>