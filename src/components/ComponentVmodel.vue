<template>
    <TextInput label="Custom label" v-model="firstName" />
    <TextInput label="Custom label2" v-model="lastName"/>
</template>

<script setup>
import { ref } from 'vue';
import TextInput from './InputText.vue';

const firstName = ref('');
const lastName = ref('');
</script>