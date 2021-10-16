<template>
  <div>
    <div v-for="(Personaje, index) of Personajes" :key="index">
      <div class="card-images">
        <img class="image-character" v-bind="Personaje" alt="Personajes" />
        <p>{{ Personaje.nombre }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "images",
  data: () => ({
    Personajes: [
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        nombre: "Morty Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
      },
      {
        nombre: "Summer Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
      },
      {
        nombre: "Beth Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
      },
      {
        nombre: "Jerry Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
      },
    ],
  }),
  
};
</script>

<style scoped>
.image-character{
  width: 120px;
  border-radius: 50%;
  margin-right: 40px;
  margin-left: 15px;
  margin-top: 10px;
}
.card-images{
  color: green;
  font-size:xx-large;
  font-weight: bold;
  -webkit-text-stroke: 0.5px white;
}
p{
  width: 50%;
  display: inline-block;
  position: absolute;
  padding-top: 20px;
}
</style>

