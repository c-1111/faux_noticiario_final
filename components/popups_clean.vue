<template>
    <div class="popups_clean_flex">
      <div class="informacion"><img src="./public/popups_clean/no_es_real.svg" alt=""></div>
      <div class="informacion2"><img src="./public/popups_clean/contenido.svg" alt=""></div>
      <div class="informacion3"><img src="./public/popups_clean/separador_euros.svg" alt=""></div>
      <div class="informacion4"><img src="./public/popups_clean/separador_estrellas.svg" alt=""></div>
    </div>
</template>

<style lang="sass">
.popups_clean_flex
    @apply flex flex-col gap-2 fixed
    .informacion
        @apply fixed bg-red-600
    .informacion2
        @apply fixed bg-red-600
    .informacion3
        @apply fixed bg-red-600
    .informacion4
        @apply fixed bg-red-600
</style>