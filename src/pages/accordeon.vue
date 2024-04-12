<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(false)
const maVar2 = ref(0)

</script>

<template>

  <p>la variable vaut : {{ maVar2 }}</p>

  <button @click="maVar2 = false ? 0 : 1">Montrer 1</button>
  <h1 v-show="maVar2 === 1" class="text-2xl">Contenu de 1</h1>

  <button @click="maVar = false">Cacher</button>

  <button @click="maVar = true">Montrer</button>

  <button @click="maVar = !maVar">Basculer</button>

  <h1 v-show="maVar" class="text-2xl">Bonjour monde !</h1>

</template>