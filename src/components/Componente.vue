<template>
  <div>
    <ul>
      <li v-for="(character, $index) in characters" :key="$index">
        <img :src="character.src" class="image"/> {{character.nombre}}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Componente',
  data: () => ({
    characters: [
      { nombre: 'Rick Sanchez', src: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg' },
      { nombre: 'Morty Smith', src: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg' },
      { nombre: 'Summer Smith', src: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg' },
      { nombre: 'Beth Smith', src: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg' },
      { nombre: 'Jerry Smith', src: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg' },
    ],
  }),
}
</script>

<style scoped>

li {
  list-style-type: none;
  display: flex;
  align-items: center;
}

.image {
  height: 100px;
  width: 100px;
  border-radius: 50%;
  padding: .5em;
}

</style>
