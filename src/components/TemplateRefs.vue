<template>
TemplateRefs.vue
<input type="text" ref="inputRef">
<div >
    <div ref="mainDiv">
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Esse, repellat voluptatum odit tenetur veritatis est dicta, nisi possimus aliquam atque nostrum nemo sint doloribus molestiae deserunt iure adipisci? Autem, debitis!</p>
    </div>
</div>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const inputRef = ref(null);

const mainDiv = ref(null);

onMounted(() => {
    console.log(mainDiv.value);
    // console.log(inputRef.value);
    inputRef.value.focus();
})
</script>