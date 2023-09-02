<template>
  <h2>Hello from App</h2>
  <Reactivity />
  <hr>
  <Computed />
</template>

<script setup>
import Reactivity from './components/Reactivity.vue';
import Computed from './components/Computed.vue';
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
