<script setup>
const name= "Lovelyn";

import { ref } from 'vue';

const count = ref(0);

function Increase() {
  count.value++;
}

const message = ref("Hello, kalibutan");

const website="https://google.com";

const color ="blue";

const isActive = true;
</script>

<template>
  <h1>{{ name }}</h1>

  <h2> {{ message }}</h2>

  {{ count }}

  <button @click="Increase">Add</button>

  <button @click="message='Hi, bebs'">Click here</button>

  <a v-bind:href="website">
    Click me
  </a>

  <p :style="{color: color}">Ooplok
  </p>

  <p :class="{active: isActive}">Sample</p>

</template>

<style>
.active{
  color: red;
  font-weight: bold;
}
</style>