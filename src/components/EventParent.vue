<template>
    <div>
        Event Parent
    </div>
    <Events @someEvent="customEventHandler"/>
</template>

<script setup>
import Events from './Events.vue';

const customEventHandler = (data) => {
    console.log(data);
}

</script>