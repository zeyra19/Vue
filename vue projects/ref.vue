<template lang="">
    <p>Count: {{count}}</p>
    <button @click="increment">Increment</button>
</template>

<script setup>
import {ref} from "vue";

const count = ref(0)
function increment() {
    count.value++
}
</script>
