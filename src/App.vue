<script setup>
const name= "Lovelyn";

import { ref } from 'vue';

const count = ref(0);

function Increase() {
  count.value++;
}

const message = ref("Hello, kalibutan");
</script>

<template>
  <h1>{{ name }}</h1>

  <h2> {{ message }}</h2>

  {{ count }}

  <button @click="Increase">Add</button>

  <button @click="message='Hi, bebs'">Click here</button>

</template>
