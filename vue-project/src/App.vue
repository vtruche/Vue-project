<script setup>
import { ref } from "vue";

const compteur = ref(0);

setInterval(() => {
  compteur.value++
}, 1000 )

function resetCompteur(){
  compteur.value = 0;
}

</script>

<template>
  <h1>Hello World</h1>
  <p>Compteur : {{compteur}}</p>
  <button v-on:click="resetCompteur()">Reset compteur</button>
  <input type="number" v-model="compteur">
</template>

<style></style>
