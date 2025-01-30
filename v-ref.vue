<template>
  <h1>
      Using Vue with TypeScript
      {{name}}
      {{user}}
  </h1>
</template>

<script setup lang="ts">
import {ref, reactive} from "vue";

interface User {
  name: string,
  age: number,
  gender: "male" | "female"
}

  const name = ref("zehra")
  name.value = "1"

  const user = reactive<User>({
    name: "Zehra",
    age: 19,
    gender: "female"
  })
</script>

<style scoped>
</style>
