<template>
    <header class="cabecalho">
    <ul class="lista">
      <div class="identificar_loja">
        <li class="logo"></li>
        <li class="nome_site"><a href="#">GameShop</a></li>
      </div>
      <li><a href="#">Ps4</a></li>
      <li><a href="#">Ps5</a></li>
      <li><a href="#">Xbox</a></li>
      <li><a href="#">Home</a></li>
      <li><a href="#">Fazer Login</a></li>
    </ul>
  </header>
</template>

<style scoped>
    .cabecalho{
    background-color: black;
    width: 100%;
}
.lista{
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}
.identificar_loja{
    display: flex;
    flex-direction: column;
    align-items: center;
    border-right: solid 1px white;
}
.nome_site{
    margin-bottom: 0.5rem;
    padding-right: 0.5rem;
}
li{
    font-size: 1.5rem;
    margin: 0 2rem;
}
.logo{
    background-image: url("https://cdn.dribbble.com/users/969279/screenshots/2367340/dark_wizard_mascot_logo.jpg");
    background-size: cover;
    background-position: center center;
    width: 3rem;
    height: 3rem;
    margin: 2rem;
}
</style>