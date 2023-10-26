<!-- <slot name="name">{{produtos?.data.attributes.jogo}}</slot>
<script setup lang="ts">
import { ref } from 'vue';
const produtos = ref(null);

fetch("https://vercel-store-kayky.vercel.app/api/jogo/1")
    .then(response => response.json())
    .then(data => produtos.value = data);
</script>

<template>
     <p>{{produtos?.data.attributes.imagem}}</p>
     <p>{{produtos?.data.attributes.jogo}}</p>
     <p>{{ produtos }}</p>
</template> -->