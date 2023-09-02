<template>
    <div>
        <h2 :class="[activeClass, errorClass]"> Class and Style Binding</h2>
        <h3 :style="isActive ? 'color: red': 'color:green'" :class="{current: isActive}">Class Binding</h3>
        <h4 :class="isActive ? 'ourcustomclass' : ''">H4</h4>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const isActive = ref(true)

const activeClass = ref('active')
const errorClass = ref('text-danger')

</script>

<style>
.active {
    color: red;
}
.text-danger {
    font-size: 20px;
}
.current {
    color: aqua;
}
</style>