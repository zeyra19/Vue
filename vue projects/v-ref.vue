<template>
  <h1>
      Using Vue with TypeScript
      {{ user.name }}
  </h1>
</template>

<script setup lang="ts">
import {ref} from "vue";

interface User {
  name: string,
  age: number,
  gender?: "male" | "female"
}

  const name = ref("zehra")
  name.value = "1"

  const user = ref<User>({
    name: "Zehra",
    age: 19,
    gender: "female"
  });
</script>

<style scoped>
</style>
