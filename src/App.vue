<template>
  <h2>Hello from App</h2>
  <!-- <Reactivity />
  <hr>
  <Computed />
  <hr>
  <ClassAndStyleBinding />
  <hr>
  <ConditionalRendering/>
  <hr>
  <ListRendering/>
  <hr> -->
  <EventHandling/>
  <InputBindings/>
</template>

<script setup>
import Reactivity from './components/Reactivity.vue';
import Computed from './components/Computed.vue';
import ClassAndStyleBinding from './components/ClassAndStyleBinding.vue';
import ConditionalRendering from './components/ConditionalRendering.vue';
import ListRendering from './components/ListRendering.vue';
import EventHandling from './components/EventHandling.vue';
import InputBindings from './components/InputBindings.vue';
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
