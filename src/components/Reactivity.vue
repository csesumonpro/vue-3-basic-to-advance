<template>
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