<template>
  <button @click="count++">Add 1</button>
    <p>Count is: {{ count }}</p>
    <input type="text" v-model="count" @keyup.b="customEvent('one', $event)" />
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)

const customEvent = (one, e) => {
  console.log('customEvent', one, e)
}
</script>
