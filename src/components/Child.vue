<template>
    <h2>From Child</h2>
    {{ props.name }}
    <br>
    {{ props.msg }}
    <br>
    {{ props.user.name }}
    <br>
    {{ props.user.age }}
    <br>
    {{ props.list }}
    <br>
    <ChildofChild abcd="abcd" :name="props.name" :childComponent="childComponent"/>
</template>

<script setup>
import ChildofChild from './ChildofChild.vue'

// const props = defineProps(['name', 'msg', 'user', 'list']);

// const props = defineProps({
//     name: String,
//     msg: String,
//     user: Object,
//     list: Array
// });

const childComponent = 'childCompoent';
const props = defineProps({
    name: {
        type: String,
        default: 'John Doe'
    },
    msg: {
        type: String,
        required: true
    },
    user: {
        type: Object,
        default: () => ({ name: 'John Doe', age: 30 })
    },
    list: {
        type: Array,
        default: () => ['Apple', 'Banana', 'Orange']
    }
})

</script>