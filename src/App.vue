<template>
    <div id="app">
        <lvBusca></lvBusca>
        <lvPerfil></lvPerfil>
    </div>
</template>

<script>
import lvBusca from './LVBusca.vue'
import lvPerfil from './LVPerfil.vue'

export default {
  name: 'App',
  components: {
   lvBusca,
   lvPerfil
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
