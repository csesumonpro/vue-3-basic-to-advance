<template>
    <div>
        <label for="name">{{props.label}}</label>
        <input type="text" id="name" v-model="fieldValue">
    </div>
</template>

<script setup>
import { computed } from 'vue';

const emit = defineEmits(['update:modelValue']);

const props = defineProps({
    label: {
        type: String,
        default: 'Name'
    },
    modelValue: {
        type: String,
        default: ''
    }
});

const fieldValue = computed({
    get: () => props.modelValue,
    set: (value) => emit('update:modelValue', value)
});


</script>