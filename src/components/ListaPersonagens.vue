<script setup>
const personagem = defineProps(["name", "status", "species", "gender","location", "episode", "url", "id"])
const imageUrl = "https://rickandmortyapi.com/api/character/avatar/"+ personagem.id + ".jpeg"


</script>

<template>
<<<<<<< HEAD
    <link rel="stylesheet" href="/src/assets/home.css">
    <div class="col-md-3">
        <div class="card md-6">
            <img :src="imageUrl" height="100%"  alt="..." class="card-img-top" >
=======
    <div class="col-md-2 ">
        <div class="card md-6">

            <img :src="imageUrl" height="150"  alt="..." class="card-img-top mt-3">
>>>>>>> be1db158649fe924aa67d78d2b69b2ab15671d30
            <h4 class="text-center">{{ personagem.name}}</h4>
            <p class="text-center"> 
                <strong> Status: </strong> {{ personagem.status }} <br>
                <strong> Raça: </strong>{{ personagem.species }}<br>
                <strong> Gênero: </strong>{{ personagem.gender }}<br>
<<<<<<< HEAD
                <strong> Localização: </strong>{{ personagem.location.name }}<br>
                <strong> Nº Episódios: </strong> {{ personagem.episode.length }}<br>
            </p>
=======
                <strong> Localização atual: </strong>{{ personagem.location.name }}<br>
                <strong> Nº Episódios: </strong> {{ personagem.episode.length }}<br>
            </p>
            
>>>>>>> be1db158649fe924aa67d78d2b69b2ab15671d30
        </div>
    </div>
</template>

<style>

</style>