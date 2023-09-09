<template>
    <ul>
        <li v-for="item in items">
            {{item}}
        </li>
    </ul>

    <ul>
        <li v-for="(item, index) in itemss">
            {{ index }}
            {{item.message}}
        </li>
    </ul>

    <ul>
        <li v-for="(item, key, index) in myObject">
            {{ key }} - 
            {{ index }} -
            {{ item }}
        </li>
    </ul>
</template>

<script setup>
import { ref, reactive } from 'vue';

const items = ref(['item1', 'item2', 'item3']);

const itemss = ref([
    { message: 'Foo' }, 
    { message: 'Bar' },
    { message: 'Baz' }
])


const myObject = reactive({
  title: 'How to do lists in Vue',
  author: 'Jane Doe',
  publishedAt: '2016-04-10'
})

</script>