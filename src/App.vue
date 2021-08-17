<template>
  <div>
    <Componente></Componente>
  </div>
</template>

<script>
import Componente from './components/Componente.vue'

export default {
  name: 'App',
  components: {
    Componente
  }
}
</script>

<style>

body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  font-weight: 700;
  color: green;
  background-image: url(https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

</style>
