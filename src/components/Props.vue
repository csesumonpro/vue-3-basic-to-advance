<template>
<h2>Props</h2>
{{ message }}
<Child :user="user" :list="fruitList"/>
</template>

<script setup>
import Child from './Child.vue'
import { ref } from 'vue'
const message = ref('Hello Vue 3!')
const user = ref({ 
    name: 'John Doe',
    age: 30
 })
const fruitList = ref(['Apple', 'Banana', 'Orange'])

</script>