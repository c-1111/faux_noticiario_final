<template>
 <div class="popups">   
    <div class="imagecontainer">
      <img v-for="(image, index) in images" :key="index" :src="image.src" :class="{ 'blinkingimage': image.blinking }" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
        { src: '/popups4/compu_paisaje.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/404.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/apple.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/arroba.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/aviso.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/cable.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/crash.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/cd.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/cd2.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/cien.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/pregunta.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/clip.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/coxis.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/cube.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/dniruso.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/molec1.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/dollar_spin.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/espacio.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/gaviota.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/giphy.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/giphy(1).gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/hoz.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/hp_giro.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/keys.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/manos.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/Mew.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/molec2.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/mouse.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/Ne12_VSH.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/ordenador_lengua.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/pda.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/portatil_rays.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/spam.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/Spin_rotation.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/stal.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/Stg44_gif_400.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/Tilt1.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/ty.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/warn_intel.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups4/warning.gif', blinking: false, top: 0, left: 0 },











        // { src: '', blinking: false , top: 0, left: 0},
      ],
    };
  },
  methods: {
    randomizeBlinking() {
      this.images.forEach((image) => {
        image.blinking = Math.random() < 0.5; // Controla si la imagen parpadea o no
      });
    },
  },
  mounted() {
    this.randomizeBlinking();
    setInterval(this.randomizeBlinking, 100); // Cambia el estado de parpadeo cada segundo
  },
};
</script>


<style scoped lang="scss">
.imagecontainer
  {
    display: grid;
    overflow-wrap: normal;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr  1fr 1fr 1fr 1fr   ;
    grid-template-rows:1fr 1fr 1fr 1fr ;
    max-width: 100vw;
    max-height: 100vh;
    overflow:visible;
    img{
      width: 150px;
    }
  }
  .blinkingimage {
    opacity: 0;
    animation: blink infinite;
  }

  @keyframes blink {
    0% {
      opacity: 0;
    }
    50% {
      opacity: 1;
    }
    100% {
      opacity: 0;
    }
  }
</style>
