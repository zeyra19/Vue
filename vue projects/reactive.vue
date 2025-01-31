<script setup>
import {reactive} from "vue";

const user=reactive({
    name: "Zehra",
    age: "19"
});

function changeAge () {
    user.age++
}
</script>

<template>
      <p>Name: {{ user.name }}</p>
      <p>Age: {{ user.age }}</p>
      <button @click="changeAge">İncrement age</button>
</template>