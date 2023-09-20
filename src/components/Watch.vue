<template>
    Watch
    <hr>
    <h2>Name: {{user.name}}</h2>
    <h2>Age: {{user.age}}</h2>
    <p>{{ email }}</p>
    <input type="email" v-model="user.info.job" />
</template>

<script setup>
import {watch, reactive, ref} from 'vue'

const email = ref('');

const user = reactive({
    name: 'John',
    age: 20,
    info: {
        job: 'Frontend',
        skills: ['html', 'css', 'js']
    }
});

watch(()=> user.info.job, (newValue, oldValue) => {
    console.log('new=>', newValue, 'old=>', oldValue);
});

</script>