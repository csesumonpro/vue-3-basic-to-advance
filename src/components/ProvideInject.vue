<template>
<p>ProvideInject</p>
<h2>{{ msg }}</h2>
<button @click="updateMessage">{{ count }}</button>
</template>

<script setup>
import { inject } from 'vue';

const {msg, updateMessage} = inject('message');
const count = inject('counter')
</script>