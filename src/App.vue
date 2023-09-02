<template>
  <h2>Hello from App</h2>
  <p>{{ name }}</p> -  {{ user.email }}
  <br/>
  <input type="text" v-model="name">
  <input type="email" v-model="user.email">
</template>

<script setup>
import { reactive, ref } from 'vue';

const name = ref('John Doe');

const user = reactive({
  name: 'John Doe',
  email: 'jon@gmail.com'
});

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
