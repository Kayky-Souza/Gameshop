<script setup lang="ts">
import { ref } from 'vue';
const produtos = ref(null);
let link = "https://vercel-store-kayky.vercel.app/api/jogo/"
fetch("https://vercel-store-kayky.vercel.app/api/jogo/")
    .then(response => response.json())
    .then(data => produtos.value = data);
</script>

<template>
    <div class="jogo" id="jogo_1">
        <img src="https://www.digiseller.ru/preview/883757/p1_3455818_84d3d06a.jpg" alt="placeholder">
        <h2>Nome do jogo</h2>
        <h2>R$ 0.00</h2>
        <h2>gênero</h2>
        <h2>ps4/ps5</h2>
        <h2>distribuidora</h2>
    </div>
</template>

<style>
    img{
    width: 150px;
    height: 200px;
}
img.imagem_destaque{
    width: 100%;
    height: 20rem;
    padding: 0;
}
.jogo{
    border-right: solid 1px black;
    border-left: solid 1px black;
    border-radius: 5px;
    margin: 2px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
}
#jogo_7,
#jogo_14{
    width: 100%;
}
@media(max-width: 940px){
    .jogo{
        width: 30vw;
    }
}
@media(max-width: 580px){
    .jogo{
        width: 45vw;
    }
}
@media(max-width: 370px){
    .jogo{
        width: 80vw;
    }
}
</style>