<template>
    <div>
        <p>FirstName: {{ user.firstName }}</p>
        <p>Full Name: {{fullName}}</p>
    </div>
</template>
<script setup>
import { reactive, computed } from 'vue';

const user = reactive({
  firstName: 'John',
  lastName: 'Doe'
});

const fullName = computed(() => {
  return `${user.firstName} ${user.lastName}`
});


</script>
