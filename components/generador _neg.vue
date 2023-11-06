<template>
  <div class="generador_neg_holder pb-4 max-[800px]:pt-6 max-[800px]:pb-12">
    <form @submit="processForm">
      <div class="generador_top">
        <div class="instruction">nombre / seudónimo</div>
        <input type="text" name="inputData">
        <div class="aviso max-w-[32ch] text-center">acepta generar una noticia que será añadida al feed</div>
      </div>
      <div class="generador_bottom">
        <button class="svg-button text-[14px]">Generar</button>
      </div>
    </form>
  </div>
</template>

<script setup>
const { inputValue } = inject("inputData") 

const processForm = (ev) => {
  ev.preventDefault()
  const inputData = ev.target.elements.inputData
  inputValue.value = inputData.value
  inputData.value = ""
}
</script>

<style lang="sass">
.generador_neg_holder 
    @apply flex flex-col items-center pt-5 font-sf bg-black text-blanco_faux
    border-bottom: solid 1px black
    form
      @apply flex flex-col items-center
      .generador_top
          @apply flex flex-col items-center 
          .instruction
              @apply flex
          input
              @apply my-2 rounded-sm border-gris200_faux text-xs p-2
              border: solid 1px 
          .aviso
              @apply text-xs px-4
      .generador_bottom
          .svg-button 
              width: 120px
              height: 50px
              background-image: url('img/fondo_boton_neg.svg') 
              fill: #fff
              background-size: 100%  // Ajusta esto según tus necesidades
              background-position-y: 50% 
              background-repeat: no-repeat
              color: #000 // Color del texto en el botón
              transform: scale(1.4)
              margin-top: .1rem
</style>