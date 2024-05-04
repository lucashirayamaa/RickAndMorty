<script setup>
  import { onMounted, reactive, ref} from 'vue';
  import ListaPersonagens from '../components/ListaPersonagens.vue';


  let personagens = reactive(ref());
  
  onMounted(() => {
    fetch("https://rickandmortyapi.com/api/character")
    .then(response => response.json())
    .then(response => {
      personagens.value = response.results
      console.log(personagens)
    })
  })

</script>

<template>
  <link rel='stylesheet' href="@/../src/assets/home.css">
  <main>
    <div class="container">
      <div class="row">
              <ListaPersonagens
              v-for="personagem in personagens"
              :key="personagem.id"
              :name="personagem.name"
              :status="personagem.status"
              :species="personagem.species"
              :gender="personagem.gender"
              :location="personagem.location"
              :episode="personagem.episode"
              :url="personagem.url"
              :id = "personagem.id"
              />
        </div>
      </div>
  </main>
</template>
