<template>
  <div class="app max-[800px]:max-w-[900px]">
    <Noticiario_header class="  bg-blanco_faux" />
    <div class="faux_grid_holder grid grid-cols-[1fr_auto_1fr] max-[800px]:grid-cols-1 max-[800px]:items-center ">
      <div class="col_lateral_1 col-span-1 ">
        <Generador @click="launch" class="sticky top-4" />
      </div>
      <div class="col_central col-span-1 max-[800px]:order-3">
        <noticiario_feed />
      </div>
      <div class="  col_lateral_2 col-span-1 max-[800px]:pl-0 max-[800px]:order-2 max-[800px]:w-full">
        <div class="link min-w-[170px] font-sf sticky top-0 border-b border-black">
          <div class="text w-full text-center flex flex-row py-4 px-8 ">
            <a href="https://faux-site.netlify.app/" class="text-center">_proyecto faux</a>
          </div>
        </div>
      </div>
    </div>
    <div class="popups_holder" v-show="showPopups1">
      <Popups1 />
    </div>
    <div class="popups_holder2" v-show="showPopups2">
      <Popups2 />
    </div>
    <div class="popups_holder3" v-show="showPopups3">
      <Popups3 />
    </div>
    <div class="popups_holder4" v-show="showPopups4">
      <Popups4 />
    </div>
    <div class="popups_holder_text" v-show="showPopupsText">
      <PopupsText />
    </div>
    <div class="popups_holder_faux" v-show="showPopupsFaux">
      <PopupsFauxFinal />
    </div>



    <prueba3 />
    <Footer />
  </div>
</template>

  
<script setup>
import { ref, onMounted } from 'vue';

const showPopups1 = ref(false);
const showPopups2 = ref(false);
const showPopups3 = ref(false);
const showPopups4 = ref(false);
const showPopupsText = ref(false);
const showPopupsFaux = ref(false);





const launch = () => {
  setTimeout(() => {
    showPopups1.value = true;
  }, 13000);
  setTimeout(() => {
    showPopups2.value = true;
  }, 19000);
  setTimeout(() => {
    showPopups3.value = true;
  }, 17000);
  setTimeout(() => {
    showPopups4.value = true;
  }, 18000);
  setTimeout(() => {
    showPopupsText.value = true;
  }, 9000);
  setTimeout(() => {
    showPopupsFaux.value = true;
  }, 22000);
};




const inputValue = ref("")
provide("inputData", {
  inputValue
})


</script>
  
<style lang="sass">
  .app
      @apply bg-white
      .popups_holder
        @apply fixed top-0 z-30 
      .popups_holder2
        @apply fixed top-0 z-20
      .popups_holder3
        @apply fixed top-0 z-10 
      .popups_holder4
        @apply fixed top-0 z-40 
      .popups_holder_text
        @apply fixed top-0 z-10
      .popups_holder_faux
        @apply fixed top-0 z-50


  </style>