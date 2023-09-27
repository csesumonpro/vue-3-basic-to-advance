<template>
  <h2 class="basic">Hello from App</h2>
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
  <!-- <EventHandling/>
  <hr>
  <InputBindings/>
  <hr>
  <LifeCycle/>
  <hr/> -->
  <!-- <Watch/>
  <hr/>
  <TemplateRefs/>
  <hr/>
  <ComponentBasic/> -->
  <Props/>
</template>

<script setup>
import Reactivity from './components/Reactivity.vue';
import Computed from './components/Computed.vue';
import ClassAndStyleBinding from './components/ClassAndStyleBinding.vue';
import ConditionalRendering from './components/ConditionalRendering.vue';
import ListRendering from './components/ListRendering.vue';
import EventHandling from './components/EventHandling.vue';
import InputBindings from './components/InputBindings.vue';
import LifeCycle from './components/LifeCycle.vue';
import Watch from './components/Watch.vue';
import TemplateRefs from './components/TemplateRefs.vue';
import ComponentBasic from './components/ComponentBasic.vue';
import Props from './components/Props.vue';
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
