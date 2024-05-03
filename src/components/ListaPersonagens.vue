<script setup>
const personagem = defineProps(["name", "status", "species", "gender","location", "episode", "url", "id"])
const imageUrl = "https://rickandmortyapi.com/api/character/avatar/"+ personagem.id + ".jpeg"


</script>

<template>
    <div class="col-md-2 ">
        <div class="card md-6">

            <img :src="imageUrl" height="150"  alt="..." class="card-img-top mt-3">
            <h4 class="text-center">{{ personagem.name}}</h4>
            <p class="text-center"> 
                <strong> Status: </strong> {{ personagem.status }} <br>
                <strong> Raça: </strong>{{ personagem.species }}<br>
                <strong> Gênero: </strong>{{ personagem.gender }}<br>
                <strong> Localização atual: </strong>{{ personagem.location.name }}<br>
                <strong> Nº Episódios: </strong> {{ personagem.episode.length }}<br>
            </p>
            
        </div>
    </div>
</template>

<style>

</style>