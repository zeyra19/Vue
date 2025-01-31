<template>
    <p>{{ name }}</p>
    <button @click="changeName">Change name</button>
</template>

<script setup lang="ts">
import {ref, reactive} from "vue";

const name = ref("zehra")

function changeName () {
    name.value = "yeni ad"
}
</script>

<style lang="">
</style>