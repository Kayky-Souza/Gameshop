<!-- {{produtos?.data.attributes.preco}} -->
<script setup lang="ts">
import { ref } from 'vue';
const produtos = ref(null);
import cabecalho from './components/cabecalho.vue';
import jogodestaque from './components/jogoDestaque.vue'
import jogo from './components/jogo.vue';
fetch("https://vercel-store-kayky.vercel.app/api/jogo/1")
    .then(response => response.json())
    .then(data => produtos.value = data);
</script>

<template>
  <cabecalho></cabecalho>
  <jogodestaque></jogodestaque>
  <div class="jogos">
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo id="jogo_7"></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo id="jogo_14"></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
    <jogo></jogo>
  </div>
</template>

<style scoped>
  .jogos{
    display: flex;
    flex-wrap: wrap;
    flex: 1;
    justify-content: space-evenly;
    margin: 1rem 0;
}

</style>

