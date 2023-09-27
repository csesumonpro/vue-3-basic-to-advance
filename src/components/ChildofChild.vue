<template>
<h2>Child of Child</h2>
{{ props.abcd }} 
<br>
{{ props.name }}
<br>
{{ props.childComponent }}
</template>

<script setup>

const props = defineProps({
    abcd: String,
    name: String,
    childComponent: String
})
</script>