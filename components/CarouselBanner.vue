<template>
  <div class="header flex">
    <p class="md:hidden">
      Envío estándar gratis a partir de 100€
    </p>
    <p class="hidden md:block">
      Envío estándar gratis en todas las compras de 100€ o más
    </p>
  </div>
</template>

<style scoped>
.header {
  overflow: hidden;
  width: 100vw;
  background-color: black;
  height: 32px;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.header p {
  color: white;
  font-family: Roboto, Roboto-fallback !important;
  text-transform: uppercase;
  letter-spacing: 1.83px;
  font-size: 10px;
  -webkit-font-smoothing: antialiased;
}
</style>
