<template>
    {{ awesome }}
    <h2 v-if="awesome">From if</h2>
    <h2 v-else>Form else</h2>
    <button @click="handleChange">Toggle</button>

    <p v-show="false">This is a p tag</p>
</template>

<script setup>
import { ref } from 'vue';
const awesome = ref(false);
const handleChange = () => {
    awesome.value = !awesome.value;
}

</script>