<script setup>
  import { onMounted, reactive, ref} from 'vue';
  import ListaPersonagens from '../components/ListaPersonagens.vue';

<<<<<<< HEAD

=======
>>>>>>> be1db158649fe924aa67d78d2b69b2ab15671d30
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
<<<<<<< HEAD
  <link rel='stylesheet' href="@/../src/assets/home.css">
  <main>
    <div class="container">
      <div class="row">
=======
  <main>
    <div class="container col-">
      <div class="row col-md-12">
          <div class="card col-md-12">
            <div class="card-body row">
>>>>>>> be1db158649fe924aa67d78d2b69b2ab15671d30
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
<<<<<<< HEAD
        </div>
      </div>
=======
            
            </div>
          </div>
        </div>
    </div>
>>>>>>> be1db158649fe924aa67d78d2b69b2ab15671d30
  </main>
</template>
