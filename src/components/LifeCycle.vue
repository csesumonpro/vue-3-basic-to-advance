<template>
    LifeCycle.vue
    {{ count }}
</template>

<script>
import { onMounted, ref} from 'vue'
export default {
    setup() {
        const count = ref(0)
        onMounted(() => {
            console.log('onMounted')
        })
        return {
            count
        }
    },
    mounted() {
        console.log('mounted')
    },

    beforeCreate() {
        console.log('beforeCreate')
    },

    created() {
        console.log('created')
    },
}
</script>